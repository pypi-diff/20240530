# Comparing `tmp/python_datapack-0.1.6.tar.gz` & `tmp/python_datapack-0.1.7.tar.gz`

## Comparing `python_datapack-0.1.6.tar` & `python_datapack-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.6/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.6/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.6/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.6/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.6/copy_in_local.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    19379 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    24338 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.6/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.6/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.6/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.6/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.7/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.1.7/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.1.7/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.1.7/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.1.7/copy_in_local.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    21133 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    26767 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.1.7/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.1.7/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.1.7/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.1.7/PKG-INFO
```

### Comparing `python_datapack-0.1.6/src/python_datapack/__init__.py` & `python_datapack-0.1.7/src/python_datapack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,22 @@
 	valid = basic_key_check(config, "resource_pack_format", int, "Resource pack format version, see https://minecraft.wiki/w/Pack_format#List_of_resource_pack_formats", valid)
 	valid = basic_key_check(config, "description", str, "Pack description displayed in pack.mcmeta", valid)
 	valid = basic_key_check(config, "dependencies", dict, "Automagically, the datapack will check for the presence of dependencies and their minimum required versions at runtime\nThe url is used when the dependency is not found to suggest where to get it\nThe version dict key contains the minimum required version of the dependency in [major, minor, patch] format\nThe main key is the dependency namespace to check for\nThe name can be whatever you want, it's just used in messages", valid)
 	valid = basic_key_check(config, "source_lore", list, "Appended lore to any custom item, can be an empty string to disable", valid)
 	has_manual = basic_key_check(config, "has_manual", bool, "Do the program generate a manual/guide? (WARNING: if an item is malformed in the database, the server log will be flooded on load by the manual hiding the malformed item)", True)
 	if has_manual == True:
 		valid = basic_key_check(config, "manual_path", str, "Cached manual assets", valid)
+		valid = basic_key_check(config, "manual_high_resolution", bool, "Enable the high resolution for the manual to increase the craft resolutions", valid)
 		valid = basic_key_check(config, "cache_manual_assets", bool, "Caches the MC assets and the items renders for the manual (manual/items/*.png)", valid)
 		valid = basic_key_check(config, "cache_manual_pages", bool, "Caches the content of the manual and the images (manual/pages/*.png)", valid)
 		valid = basic_key_check(config, "manual_debug", str, "Dump of the manual for debugging purposes", valid)
 		valid = basic_key_check(config, "manual_name", str, "Name of the manual, used for the title of the book and first page", valid)
 		valid = basic_key_check(config, "max_items_per_row", int, "Max number of items per row in the manual, should not exceed 6", valid)
 		valid = basic_key_check(config, "max_rows_per_page", int, "Max number of rows per page in the manual, should not exceed 6", valid)
-		valid = basic_key_check(config, "opengl_resolution", int, "Resolution of the OpenGL renders used in the manual, best value is 64 <--- 64x64", valid)
+		valid = basic_key_check(config, "opengl_resolution", int, "Resolution of the OpenGL renders used in the manual, best value is 256 <--- 256x256", valid)
 		valid = basic_key_check(config, "manual_first_page_text", list, "Text for the first page of the manual", valid)
 	elif valid == True:
 		valid = has_manual
 	return valid == True
 
 
 def build_process(config: dict, setup_database: callable, setup_external_database: callable = None, user_code: callable = None):
```

### Comparing `python_datapack-0.1.6/src/python_datapack/constants.py` & `python_datapack-0.1.7/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/enhance_config.py` & `python_datapack-0.1.7/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/finalyze.py` & `python_datapack-0.1.7/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/initialize.py` & `python_datapack-0.1.7/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/verify_database.py` & `python_datapack-0.1.7/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.1.7/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.1.7/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/headers.py` & `python_datapack-0.1.7/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/lang.py` & `python_datapack-0.1.7/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/loading.py` & `python_datapack-0.1.7/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.1.7/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/main.py` & `python_datapack-0.1.7/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/datapack/recipes.py` & `python_datapack-0.1.7/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.1.7/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/main.py` & `python_datapack-0.1.7/src/python_datapack/manual/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Imports
 from ..utils.io import *
 from ..utils.print import *
 from .utils import *
 from .shared_import import *
 from .book_optimizer import *
 from ..constants import *
+from copy import deepcopy
 
 def main(config: dict):
 
 	# Prework
 	os.makedirs(f"{config['manual_path']}/font/page", exist_ok=True)
 	os.makedirs(f"{config['manual_path']}/font/wiki_icons", exist_ok = True)
 	generate_all_iso_renders(config)
@@ -25,15 +26,18 @@
 	if not config['debug_mode']:
 		super_copy(f"{TEMPLATES_PATH}/none_release.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
 	else:
 		super_copy(f"{TEMPLATES_PATH}/none.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/none.png")
 	super_copy(f"{TEMPLATES_PATH}/wiki_information.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_information.png")
 	super_copy(f"{TEMPLATES_PATH}/wiki_result_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_result_of_craft.png")
 	super_copy(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_ingredient_of_craft.png")
-
+	if config['manual_high_resolution']:
+		super_copy(f"{TEMPLATES_PATH}/furnace.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/furnace.png")
+		super_copy(f"{TEMPLATES_PATH}/shaped_2x2.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/shaped_2x2.png")
+		super_copy(f"{TEMPLATES_PATH}/shaped_3x3.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/shaped_3x3.png")
 
 	# If the manual cache is enabled and we have a cache file, load it
 	if config['cache_manual_pages'] and os.path.exists(config['manual_debug']):
 		with super_open(config['manual_debug'], "r") as f:
 			book_content = json.load(f)
 
 	# Else, generate all
@@ -88,15 +92,15 @@
 		for item, data in sorted_database_on_category:
 			i += 1
 			manual_pages.append({"number": i, "name": item, "raw_data": data, "type": "item"})
 
 		# Encode pages
 		book_content = []
 		os.makedirs(f"{config['manual_path']}/font/category", exist_ok=True)
-		simple_case = Image.open(f"{TEMPLATES_PATH}/simple_case_no_border.png")	# Load the simple case image for later use in categories pages
+		simple_case = load_simple_case_no_border(config['manual_high_resolution'])	# Load the simple case image for later use in categories pages
 		for page in manual_pages:
 			content = []
 			number = page["number"]
 			page_font = get_page_font(number)
 			name = str(page["name"])
 			raw_data = page["raw_data"]
 			titled = name.replace("_", " ").title() + "\n"
@@ -113,46 +117,55 @@
 				# Prepare image and line list
 				page_image = Image.new("RGBA", (256, 256), (0, 0, 0, 0))
 				x, y = 2, 2	# Prevision for global border and implicit border
 				line = []
 
 				# For each item in the category, get its page number and texture, then add it to the image
 				for item in raw_data:
+
+					# Get item texture
 					texture_path = f"{config['manual_path']}/items/{config['namespace']}/{item}.png"
 					if os.path.exists(texture_path):
 						item_image = Image.open(texture_path)
 					else:
 						warning(f"Missing texture at '{texture_path}', using empty texture")
-						item_image = Image.new("RGBA", (16, 16), (0, 0, 0, 0))
-					factor = 32 / item_image.size[0]
-					item_image = item_image.resize((32, int(item_image.size[1] * factor)), Image.NEAREST)
+						item_image = Image.new("RGBA", (1, 1), (0, 0, 0, 0))
+					if not config['manual_high_resolution']:
+						resized = careful_resize(item_image, 32)
+					else:
+						resized = Image.new("RGBA", (1, 1), (0, 0, 0, 0))	# Empty texture to use for category page
+						high_res_font = generate_high_res_font(config, item, item_image)
 
 					# Paste the simple case and the item_image
 					page_image.paste(simple_case, (x, y))
-					mask = item_image.convert("RGBA").split()[3]
-					page_image.paste(item_image, (x + 2, y + 2), mask)
-					x += 36
+					mask = resized.convert("RGBA").split()[3]
+					page_image.paste(resized, (x + 2, y + 2), mask)
+					x += simple_case.size[0]
 
 					# Add the clickEvent part to the line and add the 2 times the line if enough items
 					component = get_item_component(config, item, ["custom_model_data", "item_name", "custom_name"])
-					component["text"] = MEDIUM_NONE_FONT
+					component["text"] = MEDIUM_NONE_FONT if not config['manual_high_resolution'] else high_res_font
 					line.append(component)
 					if len(line) == config['max_items_per_row']:
-						line[-1]["text"] += "\n"
-						line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
-						content += line * 2
+						line.insert(0, SMALL_NONE_FONT * LEFT_PADDING)
+						content += deepcopy(line)
+						for i in range(1, len(line)):
+							line[-i]["text"] = MEDIUM_NONE_FONT
+						content += ["\n"] + line + ["\n"]
 						line = []
 						x = 2
-						y += 36
+						y += simple_case.size[1]
 				
 				# If remaining items in the line, add them
 				if len(line) > 0:
-					line[-1]["text"] += "\n"
-					line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
-					content += line * 2
+					line.insert(0, SMALL_NONE_FONT * LEFT_PADDING)
+					content += deepcopy(line)
+					for i in range(1, len(line)):
+						line[-i]["text"] = MEDIUM_NONE_FONT
+					content += ["\n"] + line + ["\n"]
 				
 				# Add the 2 pixels border
 				is_rectangle_shape = len(raw_data) % config['max_items_per_row'] == 0
 				page_image = add_border(page_image, BORDER_COLOR, BORDER_SIZE, is_rectangle_shape)
 				
 				# Save the image
 				page_image.save(f"{config['manual_path']}/font/category/{file_name}.png")
@@ -297,36 +310,48 @@
 
 		# For each item in the category, get its page number and texture, then add it to the image
 		for page in manual_pages:
 			if page["type"] == CATEGORY:
 				item = page["raw_data"][0]
 				texture_path = f"{config['manual_path']}/items/{config['namespace']}/{item}.png"
 				item_image = Image.open(texture_path)
-				factor = 32 / item_image.size[0]
-				item_image = item_image.resize((32, int(item_image.size[1] * factor)), Image.NEAREST)
+				item_image = careful_resize(item_image, 32)
+
+				# Get item texture
+				texture_path = f"{config['manual_path']}/items/{config['namespace']}/{item}.png"
+				if os.path.exists(texture_path):
+					item_image = Image.open(texture_path)
+				else:
+					warning(f"Missing texture at '{texture_path}', using empty texture")
+					item_image = Image.new("RGBA", (1, 1), (0, 0, 0, 0))
+				if not config['manual_high_resolution']:
+					resized = careful_resize(item_image, 32)
+				else:
+					resized = Image.new("RGBA", (1, 1), (0, 0, 0, 0))	# Empty texture to use for category page
+					high_res_font = generate_high_res_font(config, item, item_image)
 
 				# Paste the simple case and the item_image
 				page_image.paste(simple_case, (x, y))
 				mask = item_image.convert("RGBA").split()[3]
 				page_image.paste(item_image, (x + 2, y + 2), mask)
-				x += 36
+				x += simple_case.size[0]
 
 				# Add the clickEvent part to the line and add the 2 times the line if enough items
 				component = get_item_component(config, item, ["custom_model_data"])
 				component["hoverEvent"]["contents"]["components"]["item_name"] = str({"text": page["name"], "color": "white"})
 				component["clickEvent"]["value"] = str(page["number"])
 				component["text"] = MEDIUM_NONE_FONT
 				line.append(component)
 				if len(line) == config['max_items_per_row']:
 					line[-1]["text"] += "\n"
 					line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
 					content += line * 2
 					line = []
 					x = 2
-					y += 36
+					y += simple_case.size[1]
 		
 		# If remaining items in the line, add them
 		if len(line) > 0:
 			line[-1]["text"] += "\n"
 			line[0]["text"] = SMALL_NONE_FONT * LEFT_PADDING + line[0]["text"]
 			content += line * 2
 		
@@ -347,15 +372,15 @@
 		content.append({"text": MEDIUM_NONE_FONT * 2 + page_font, "font": FONT, "color": "white"})
 		
 		# Create the image and load Minecraft font
 		icon_path = f"{config['assets_folder']}/original_icon.png"
 		if not os.path.exists(icon_path):
 			error(f"Missing icon path at '{icon_path}' (needed for the manual)")
 		logo = Image.open(icon_path)
-		logo = logo.resize((256, 256), Image.NEAREST)
+		logo = careful_resize(logo, 256)
 
 		# Write the introduction text
 		content.append("\n" * 6)
 		content.append(config['manual_first_page_text'])
 
 		# Save image and insert in the manual pages
 		logo.save(f"{config['manual_path']}/font/page/_logo.png")
@@ -365,14 +390,15 @@
 		book_content = optimize_book(book_content)
 
 		# Add fonts
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 8, "height": 20, "chars": [NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 8, "height": 18, "chars": [MEDIUM_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 7, "height": 7, "chars": [SMALL_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 0, "height": 2, "chars": [VERY_SMALL_NONE_FONT]})
+		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 0, "height": 1, "chars": [MICRO_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/none.png", "ascent": 7, "height": 16, "chars": [WIKI_NONE_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_information.png", "ascent": 8, "height": 16, "chars": [WIKI_INFO_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_result_of_craft.png", "ascent": 8, "height": 16, "chars": [WIKI_RESULT_OF_CRAFT_FONT]})
 		font_providers.append({"type":"bitmap","file":f"{config['namespace']}:font/wiki_ingredient_of_craft.png", "ascent": 8, "height": 16, "chars": [WIKI_INGR_OF_CRAFT_FONT]})
 		fonts = {"providers": font_providers}
 		with super_open(f"{config['manual_path']}/font/manual.json", "w") as f:
 			f.write(super_json_dump(fonts).replace("\\\\", "\\"))
@@ -384,14 +410,16 @@
 
 
 	# Copy the font provider and the generated textures to the resource pack
 	super_copy(f"{config['manual_path']}/font/manual.json", f"{config['build_resource_pack']}/assets/{config['namespace']}/font/manual.json")
 	super_copy(f"{config['manual_path']}/font/category/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/category/")
 	super_copy(f"{config['manual_path']}/font/page/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/page/")
 	super_copy(f"{config['manual_path']}/font/wiki_icons/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_icons/")
+	if config['manual_high_resolution']:
+		super_copy(f"{config['manual_path']}/font/high_res/", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/high_res/")
 
 
 	# Finally, prepend the manual to the database
 	manual_cmd = min(x["custom_model_data"] for x in config['database'].values() if x.get("custom_model_data")) - 1		# First custom_model_data minus 1
 	manual_database = {"manual":
 		{
 			"id": "minecraft:written_book",
```

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/shared_import.py` & `python_datapack-0.1.7/src/python_datapack/manual/shared_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 BORDER_COLOR = 0xB64E2F
 BORDER_COLOR = (BORDER_COLOR >> 16) & 0xFF, (BORDER_COLOR >> 8) & 0xFF, BORDER_COLOR & 0xFF, 255
 BORDER_SIZE = 2
 NONE_FONT = get_font(0x0000)
 MEDIUM_NONE_FONT = get_font(0x0001)
 SMALL_NONE_FONT = get_font(0x0002)
 VERY_SMALL_NONE_FONT = get_font(0x0003)
-WIKI_NONE_FONT = get_font(0x0004)
-WIKI_INFO_FONT = get_font(0x0005)
-WIKI_RESULT_OF_CRAFT_FONT = get_font(0x0006)
-WIKI_INGR_OF_CRAFT_FONT = get_font(0x0007)
+MICRO_NONE_FONT = get_font(0x0004)
+WIKI_NONE_FONT = get_font(0x0005)
+WIKI_INFO_FONT = get_font(0x0006)
+WIKI_RESULT_OF_CRAFT_FONT = get_font(0x0007)
+WIKI_INGR_OF_CRAFT_FONT = get_font(0x0008)
 
 # Global variables
 next_craft_font = 0x8000
 font_providers = []
 manual_pages = []
 
 # Get page number
```

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/utils.py` & `python_datapack-0.1.7/src/python_datapack/manual/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,47 @@
 from ..constants import *
 from .shared_import import *
 from pathlib import Path
 from PIL import Image, ImageDraw, ImageFont
 from model_resolver.cli import main as model_resolver_main
 import requests
 
+# Generate high res simple case no border
+def load_simple_case_no_border(high_res: bool) -> Image.Image:
+	path = f"{TEMPLATES_PATH}/simple_case_no_border.png"
+	img = Image.open(path)
+	if not high_res:
+		return img
+
+	# Make the image bigger on the right
+	middle_x = img.size[0] // 2
+	result = Image.new("RGBA", (img.size[0] + 1, img.size[1]))
+	result.paste(img, (0, 0))
+	img = img.crop((middle_x, 0, img.size[0], img.size[1]))
+	result.paste(img, (middle_x + 1, 0))
+	return result
+
+# Careful resize
+def careful_resize(image: Image.Image, max_result_size: int) -> Image.Image:
+	""" Resize an image while keeping the aspect ratio.\n
+	Example 1: if the image is 100x200 and the max_result_size is 150, the result will be 75x150.\n
+	Example 2: if the image is 200x100 and the max_result_size is 256, the result will be 256x128.\n
+	Args:
+		image			(Image):	The image to resize
+		max_result_size	(int):		The minimum result size of the image (ex: 256)
+	Returns:
+		Image: The resized image
+	"""
+	if image.size[0] >= image.size[1]:
+		factor = max_result_size / image.size[0]
+		return image.resize((max_result_size, int(image.size[1] * factor)), Image.NEAREST)
+	else:
+		factor = max_result_size / image.size[1]
+		return image.resize((int(image.size[0] * factor), max_result_size), Image.NEAREST)
+
 # Generate a border for a given Image
 def add_border(image: Image.Image, border_color: tuple, border_size: int, is_rectangle_shape: bool) -> Image.Image:
 	""" Add a border to every part of the image
 	Args:
 		image				(Image):	The image to add the border
 		border_color		(tuple):	The color of the border
 		border_size			(int):		The size of the border
@@ -57,15 +90,15 @@
 		border.paste(image, (0, 0), image)
 		image.paste(border, (0, 0), border)
 	
 	# Return the image
 	return image
 
 # Generate an image showing the result count
-def image_count(count: int) -> Image:
+def image_count(count: int) -> Image.Image:
 	""" Generate an image showing the result count
 	Args:
 		count (int): The count to show
 	Returns:
 		Image: The image with the count
 	"""
 	# Create the image
@@ -73,16 +106,16 @@
 	draw = ImageDraw.Draw(img)
 	font_size = 16
 	font = ImageFont.truetype(f"{TEMPLATES_PATH}/minecraft_font.ttf", size = font_size)
 
 	# Calculate text size and positions of the two texts
 	text_width = draw.textlength(str(count), font = font)
 	text_height = font_size + 4
-	pos_1 = (32-text_width), (32-text_height)
-	pos_2 = (30-text_width), (30-text_height)
+	pos_1 = (34-text_width), (32-text_height)
+	pos_2 = (32-text_width), (30-text_height)
 	
 	# Draw the count
 	draw.text(pos_1, str(count), (50, 50, 50), font = font)
 	draw.text(pos_2, str(count), (255, 255, 255), font = font)
 	return img
 
 # Generate iso renders for every item in the config['database']
@@ -152,15 +185,14 @@
 		destination = f"{path}/minecraft/{item}.png"
 		if not (os.path.exists(destination) and config['cache_manual_assets']):	# If not downloaded yet or not using cache
 			debug(f"Downloading texture for item '{item}'...")
 			response = requests.get(f"{DOWNLOAD_VANILLA_ASSETS_RAW}/item/{item}.png")
 			if response.status_code == 200:
 				with super_open(destination, "wb") as file:
 					file.write(response.content)
-				debug(f"Downloaded texture for item '{item}'!")
 			else:
 				warning(f"Failed to download texture for item '{item}', please add it manually to '{destination}'")
 				warning(f"Suggestion link: '{DOWNLOAD_VANILLA_ASSETS_SOURCE}'")
 		pass
 	debug("Downloaded all the vanilla textures, or using cached ones")
 
 
@@ -188,19 +220,15 @@
 	if craft and craft.get("result"):
 		result_id = ingr_to_id(craft["result"])
 		result_id = result_id.replace(":", "/")
 		image_path = f"{config['manual_path']}/items/{result_id}.png"
 		result_texture = Image.open(image_path)
 
 	# Resize the texture and get the mask
-	factor = SQUARE_SIZE / result_texture.size[0]
-	result_texture = result_texture.resize(
-		(int(result_texture.size[0]*factor), int(result_texture.size[1]*factor)),
-		Image.NEAREST
-	)
+	result_texture = careful_resize(result_texture, SQUARE_SIZE)
 	result_mask = result_texture.convert("RGBA").split()[3]
 	
 	# Check if there is a craft
 	if craft:
 
 		# Shaped craft
 		if craft["type"] in "crafting_shaped":
@@ -225,19 +253,15 @@
 						
 						# Get the texture and place it at the coords
 						item = item.replace(":", "/")
 						image_path = f"{config['manual_path']}/items/{item}.png"
 						if not os.path.exists(image_path):
 							error(f"Missing item texture at '{image_path}'")
 						item_texture = Image.open(image_path)
-						factor = SQUARE_SIZE / item_texture.size[0]
-						item_texture = item_texture.resize(
-							(int(item_texture.size[0]*factor), int(item_texture.size[1]*factor)),
-							Image.NEAREST
-						)
+						item_texture = careful_resize(item_texture, SQUARE_SIZE)
 						coords = (
 							j * (SQUARE_SIZE + CASE_OFFSETS[0]) + STARTING_PIXEL[0],
 							i * (SQUARE_SIZE + CASE_OFFSETS[1]) + STARTING_PIXEL[1]
 						)
 						mask = item_texture.convert("RGBA").split()[3]
 						template.paste(item_texture, coords, mask)
 			
@@ -263,19 +287,15 @@
 			# Place input item
 			input_item = ingr_to_id(craft["ingredient"])
 			input_item = input_item.replace(":", "/")
 			image_path = f"{config['manual_path']}/items/{input_item}.png"
 			if not os.path.exists(image_path):
 				error(f"Missing item texture at '{image_path}'")
 			item_texture = Image.open(image_path)
-			factor = SQUARE_SIZE / item_texture.size[0]
-			item_texture = item_texture.resize(
-				(int(item_texture.size[0]*factor), int(item_texture.size[1]*factor)),
-				Image.NEAREST
-			)
+			item_texture = careful_resize(item_texture, SQUARE_SIZE)
 			mask = item_texture.convert("RGBA").split()[3]
 			template.paste(item_texture, (4, 4), mask)
 
 			# Place the result item and count if the result is greater than 1
 			coords = (124, 40)
 			template.paste(result_texture, coords, result_mask)
 			if craft["result_count"] > 1:
@@ -590,15 +610,15 @@
 		texture_path = f"{config['manual_path']}/items/{result_item}.png"
 		result_item = result_item.replace("/", "_")
 		dest_path = f"{config['manual_path']}/font/wiki_icons/{result_item}.png"
 		if not os.path.exists(dest_path):
 
 			# Load texture and resize it
 			item_texture = Image.open(texture_path)
-			item_texture = item_texture.resize((42, 42), Image.NEAREST)
+			item_texture = careful_resize(item_texture, 42)
 			item_texture = item_texture.convert("RGBA")
 
 			# Load the template and paste the texture on it
 			template = Image.open(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft_template.png")
 			template.paste(item_texture, (11, 11), item_texture)
 			
 			# Save the result
@@ -611,7 +631,52 @@
 	except Exception as e:
 		warning(f"Failed to generate craft icon for {name}: {e}\nreturning default font...")
 		pass
 
 	# Return the font
 	return font
 
+# Generate high res image for item
+def generate_high_res_font(config: dict, item: str, item_image: Image.Image, count: int = 1) -> str:
+	""" Generate the high res font to display in the manual for the item
+	Args:
+		item		(str):		The name of the item, ex: "adamantium_fragment"
+		item_image	(Image):	The image of the item
+		count		(int):		The count of the item
+	Returns:
+		str: The font to the generated texture
+	"""
+	font = get_next_font()
+	item = f"{item}_{count}" if count > 1 else item
+	
+	# Get output path
+	path = f"{config['manual_path']}/font/high_res/{item}.png"
+	provider_path = f"{config['namespace']}:font/high_res/{item}.png"
+	for p in font_providers:	# Check if it already exists
+		if p["file"] == provider_path:
+			return p["chars"][0]
+	font_providers.append({"type":"bitmap","file": provider_path, "ascent": 7, "height": 16, "chars": [font]})
+
+
+	# Generate high res font
+	os.makedirs(os.path.dirname(path), exist_ok = True)
+	high_res: int = 256
+	resized = careful_resize(item_image, high_res)
+	resized = resized.convert("RGBA")
+
+	# Add the item count
+	if count > 1:
+		img_count = image_count(count)
+		img_count = careful_resize(img_count, high_res)
+		resized.paste(img_count, (0, 0), img_count)
+
+	# Add invisible pixels for minecraft font at each corner
+	total_width = resized.size[0] - 1
+	total_height = resized.size[1] - 1
+	angles = [(0, 0), (total_width, 0), (0, total_height), (total_width, total_height)]
+	for angle in angles:
+		resized.putpixel(angle, (0, 0, 0, 100))
+
+	# Save the result and return the font
+	resized.save(path)
+	return MICRO_NONE_FONT + font
+
```

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.1.7/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.1.7/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.1.7/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.1.7/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/resource_pack/main.py` & `python_datapack-0.1.7/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.1.7/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.1.7/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/utils/database_helper.py` & `python_datapack-0.1.7/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/utils/ingredients.py` & `python_datapack-0.1.7/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/utils/io.py` & `python_datapack-0.1.7/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.1.7/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/utils/print.py` & `python_datapack-0.1.7/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/src/python_datapack/utils/weld.py` & `python_datapack-0.1.7/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/LICENSE` & `python_datapack-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.1.6/pyproject.toml` & `python_datapack-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.1.6/PKG-INFO` & `python_datapack-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

