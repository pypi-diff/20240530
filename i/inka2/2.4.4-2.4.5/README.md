# Comparing `tmp/inka2-2.4.4.tar.gz` & `tmp/inka2-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inka2-2.4.4.tar", last modified: Sat Mar  9 17:17:54 2024, max compression
+gzip compressed data, was "inka2-2.4.5.tar", last modified: Thu May 30 10:18:40 2024, max compression
```

## Comparing `inka2-2.4.4.tar` & `inka2-2.4.5.tar`

### file list

```diff
@@ -1,57 +1,56 @@
--rw-r--r--   0        0        0    35149 2023-08-04 16:36:52.819506 inka2-2.4.4/LICENSE
--rw-r--r--   0        0        0     4677 2024-02-25 09:41:49.329179 inka2-2.4.4/README.md
--rw-r--r--   0        0        0     3107 2024-03-09 17:17:54.004636 inka2-2.4.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-09 17:17:28.423877 inka2-2.4.4/src/inka2/__init__.py
--rw-r--r--   0        0        0       75 2023-08-04 16:36:52.822682 inka2-2.4.4/src/inka2/__main__.py
--rw-r--r--   0        0        0    17815 2024-03-09 17:16:35.733436 inka2-2.4.4/src/inka2/cli.py
--rw-r--r--   0        0        0      239 2024-02-25 18:11:51.310582 inka2-2.4.4/src/inka2/config.ini
--rw-r--r--   0        0        0      275 2024-02-24 13:14:09.534245 inka2-2.4.4/src/inka2/exceptions.py
--rw-r--r--   0        0        0      428 2024-03-09 14:29:21.507133 inka2-2.4.4/src/inka2/hashes.json
--rw-r--r--   0        0        0     1146 2024-02-25 17:25:12.902782 inka2-2.4.4/src/inka2/helpers.py
--rw-r--r--   0        0        0        0 2023-08-04 16:36:52.823903 inka2-2.4.4/src/inka2/mistune_plugins/__init__.py
--rw-r--r--   0        0        0      912 2023-08-04 16:36:52.824374 inka2-2.4.4/src/inka2/mistune_plugins/mathjax.py
--rw-r--r--   0        0        0        0 2023-08-04 16:36:52.824891 inka2-2.4.4/src/inka2/models/__init__.py
--rw-r--r--   0        0        0     8089 2024-03-02 09:32:09.947532 inka2-2.4.4/src/inka2/models/anki_api.py
--rw-r--r--   0        0        0     2326 2024-03-09 17:07:24.822407 inka2-2.4.4/src/inka2/models/anki_media.py
--rw-r--r--   0        0        0     3522 2024-02-25 16:50:57.799631 inka2-2.4.4/src/inka2/models/config.py
--rw-r--r--   0        0        0     4765 2024-02-25 14:34:08.389753 inka2-2.4.4/src/inka2/models/converter.py
--rw-r--r--   0        0        0     1318 2023-08-04 16:36:52.826224 inka2-2.4.4/src/inka2/models/hasher.py
--rw-r--r--   0        0        0     5994 2023-08-04 16:36:52.826469 inka2-2.4.4/src/inka2/models/highlighter.py
--rw-r--r--   0        0        0     4600 2024-03-09 17:07:24.778031 inka2-2.4.4/src/inka2/models/img_handler.py
--rw-r--r--   0        0        0        0 2023-08-04 16:36:52.827088 inka2-2.4.4/src/inka2/models/notes/__init__.py
--rw-r--r--   0        0        0     3399 2024-02-25 17:25:12.903265 inka2-2.4.4/src/inka2/models/notes/basic_note.py
--rw-r--r--   0        0        0     2860 2024-02-25 17:25:12.903928 inka2-2.4.4/src/inka2/models/notes/cloze_note.py
--rw-r--r--   0        0        0     2512 2024-02-25 17:25:12.902732 inka2-2.4.4/src/inka2/models/notes/note.py
--rw-r--r--   0        0        0     8825 2024-02-25 17:25:12.907442 inka2-2.4.4/src/inka2/models/parser.py
--rw-r--r--   0        0        0     5829 2024-03-09 17:13:52.247843 inka2-2.4.4/src/inka2/models/writer.py
--rw-r--r--   0        0        0     3765 2024-02-25 17:25:12.903285 inka2-2.4.4/tests/conftest.py
--rw-r--r--   0        0        0     3807 2023-08-04 16:36:52.829185 inka2-2.4.4/tests/parser/test_get_cleaned_answer.py
--rw-r--r--   0        0        0     1185 2023-08-04 16:36:52.829816 inka2-2.4.4/tests/parser/test_get_deck_name.py
--rw-r--r--   0        0        0     1088 2023-08-04 16:36:52.830078 inka2-2.4.4/tests/parser/test_get_id.py
--rw-r--r--   0        0        0     7696 2023-08-04 16:36:52.830335 inka2-2.4.4/tests/parser/test_get_note_strings.py
--rw-r--r--   0        0        0     7093 2024-02-25 17:25:12.902945 inka2-2.4.4/tests/parser/test_get_notes_from_section.py
--rw-r--r--   0        0        0     3805 2023-08-04 16:36:52.830996 inka2-2.4.4/tests/parser/test_get_question.py
--rw-r--r--   0        0        0      919 2023-08-04 16:36:52.831230 inka2-2.4.4/tests/parser/test_get_sections.py
--rw-r--r--   0        0        0      930 2023-08-04 16:36:52.831455 inka2-2.4.4/tests/parser/test_get_tags.py
--rw-r--r--   0        0        0     1785 2023-08-04 16:36:52.831703 inka2-2.4.4/tests/parser/test_is_basic_note_str.py
--rw-r--r--   0        0        0     1786 2023-08-04 16:36:52.831959 inka2-2.4.4/tests/parser/test_is_cloze_note_str.py
--rw-r--r--   0        0        0      187 2024-02-24 09:57:31.256941 inka2-2.4.4/tests/resources/anki_data/README.txt
--rw-r--r--   0        0        0        0 2024-02-24 09:57:17.199383 inka2-2.4.4/tests/resources/anki_data/anki.log
--rw-r--r--   0        0        0    12288 2024-02-24 12:38:03.251271 inka2-2.4.4/tests/resources/anki_data/prefs21.db
--rw-r--r--   0        0        0      235 2024-02-25 17:01:31.224559 inka2-2.4.4/tests/resources/defaults/config_add_filename.ini
--rw-r--r--   0        0        0      843 2024-03-09 16:46:50.071416 inka2-2.4.4/tests/resources/index_out_of_range.md
--rw-r--r--   0        0        0      322 2024-02-24 12:40:05.719614 inka2-2.4.4/tests/resources/test_inka_data.md
--rw-r--r--   0        0        0      209 2024-02-24 11:13:15.265549 inka2-2.4.4/tests/resources/test_inka_data_init.md
--rw-r--r--   0        0        0     2203 2023-08-04 16:36:52.832225 inka2-2.4.4/tests/test_anki_media.py
--rw-r--r--   0        0        0     2567 2024-02-25 14:31:45.346757 inka2-2.4.4/tests/test_basic_note.py
--rw-r--r--   0        0        0      878 2024-03-09 16:47:47.027857 inka2-2.4.4/tests/test_cli.py
--rw-r--r--   0        0        0     2202 2024-02-25 14:32:33.200106 inka2-2.4.4/tests/test_cloze_note.py
--rw-r--r--   0        0        0     4651 2024-02-25 16:50:57.796797 inka2-2.4.4/tests/test_config.py
--rw-r--r--   0        0        0    14246 2024-02-25 17:25:12.679899 inka2-2.4.4/tests/test_converter.py
--rw-r--r--   0        0        0     3106 2024-02-24 13:13:12.907154 inka2-2.4.4/tests/test_hasher.py
--rw-r--r--   0        0        0     1986 2024-02-25 14:34:40.980287 inka2-2.4.4/tests/test_helpers.py
--rw-r--r--   0        0        0     9929 2024-02-24 13:13:12.805258 inka2-2.4.4/tests/test_highlight.py
--rw-r--r--   0        0        0     8190 2024-02-24 13:13:12.888067 inka2-2.4.4/tests/test_img_handler.py
--rw-r--r--   0        0        0      794 2024-02-24 13:13:12.840246 inka2-2.4.4/tests/test_note.py
--rw-r--r--   0        0        0    21422 2024-03-09 15:01:49.185282 inka2-2.4.4/tests/test_writer.py
--rw-r--r--   0        0        0     5836 1970-01-01 00:00:00.000000 inka2-2.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 16:36:52.819506 inka2-2.4.5/LICENSE
+-rw-r--r--   0        0        0     4677 2024-02-25 09:41:49.329179 inka2-2.4.5/README.md
+-rw-r--r--   0        0        0     3107 2024-05-30 10:18:40.334607 inka2-2.4.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-30 10:17:52.361268 inka2-2.4.5/src/inka2/__init__.py
+-rw-r--r--   0        0        0       75 2023-08-04 16:36:52.822682 inka2-2.4.5/src/inka2/__main__.py
+-rw-r--r--   0        0        0    17892 2024-03-10 09:17:53.068932 inka2-2.4.5/src/inka2/cli.py
+-rw-r--r--   0        0        0      239 2024-05-30 10:15:51.963090 inka2-2.4.5/src/inka2/config.ini
+-rw-r--r--   0        0        0      275 2024-02-24 13:14:09.534245 inka2-2.4.5/src/inka2/exceptions.py
+-rw-r--r--   0        0        0     1146 2024-02-25 17:25:12.902782 inka2-2.4.5/src/inka2/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:36:52.823903 inka2-2.4.5/src/inka2/mistune_plugins/__init__.py
+-rw-r--r--   0        0        0      912 2023-08-04 16:36:52.824374 inka2-2.4.5/src/inka2/mistune_plugins/mathjax.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:36:52.824891 inka2-2.4.5/src/inka2/models/__init__.py
+-rw-r--r--   0        0        0     8375 2024-05-30 10:15:20.292931 inka2-2.4.5/src/inka2/models/anki_api.py
+-rw-r--r--   0        0        0     2326 2024-03-09 17:27:58.452564 inka2-2.4.5/src/inka2/models/anki_media.py
+-rw-r--r--   0        0        0     3522 2024-02-25 16:50:57.799631 inka2-2.4.5/src/inka2/models/config.py
+-rw-r--r--   0        0        0     4765 2024-02-25 14:34:08.389753 inka2-2.4.5/src/inka2/models/converter.py
+-rw-r--r--   0        0        0     1318 2023-08-04 16:36:52.826224 inka2-2.4.5/src/inka2/models/hasher.py
+-rw-r--r--   0        0        0     5994 2023-08-04 16:36:52.826469 inka2-2.4.5/src/inka2/models/highlighter.py
+-rw-r--r--   0        0        0     4619 2024-03-10 09:17:53.068114 inka2-2.4.5/src/inka2/models/img_handler.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:36:52.827088 inka2-2.4.5/src/inka2/models/notes/__init__.py
+-rw-r--r--   0        0        0     3399 2024-02-25 17:25:12.903265 inka2-2.4.5/src/inka2/models/notes/basic_note.py
+-rw-r--r--   0        0        0     2860 2024-02-25 17:25:12.903928 inka2-2.4.5/src/inka2/models/notes/cloze_note.py
+-rw-r--r--   0        0        0     2512 2024-02-25 17:25:12.902732 inka2-2.4.5/src/inka2/models/notes/note.py
+-rw-r--r--   0        0        0     8825 2024-02-25 17:25:12.907442 inka2-2.4.5/src/inka2/models/parser.py
+-rw-r--r--   0        0        0     5898 2024-03-10 09:17:53.068603 inka2-2.4.5/src/inka2/models/writer.py
+-rw-r--r--   0        0        0     3765 2024-02-25 17:25:12.903285 inka2-2.4.5/tests/conftest.py
+-rw-r--r--   0        0        0     3807 2023-08-04 16:36:52.829185 inka2-2.4.5/tests/parser/test_get_cleaned_answer.py
+-rw-r--r--   0        0        0     1185 2023-08-04 16:36:52.829816 inka2-2.4.5/tests/parser/test_get_deck_name.py
+-rw-r--r--   0        0        0     1088 2023-08-04 16:36:52.830078 inka2-2.4.5/tests/parser/test_get_id.py
+-rw-r--r--   0        0        0     7696 2023-08-04 16:36:52.830335 inka2-2.4.5/tests/parser/test_get_note_strings.py
+-rw-r--r--   0        0        0     7093 2024-02-25 17:25:12.902945 inka2-2.4.5/tests/parser/test_get_notes_from_section.py
+-rw-r--r--   0        0        0     3805 2023-08-04 16:36:52.830996 inka2-2.4.5/tests/parser/test_get_question.py
+-rw-r--r--   0        0        0      919 2023-08-04 16:36:52.831230 inka2-2.4.5/tests/parser/test_get_sections.py
+-rw-r--r--   0        0        0      930 2023-08-04 16:36:52.831455 inka2-2.4.5/tests/parser/test_get_tags.py
+-rw-r--r--   0        0        0     1785 2023-08-04 16:36:52.831703 inka2-2.4.5/tests/parser/test_is_basic_note_str.py
+-rw-r--r--   0        0        0     1786 2023-08-04 16:36:52.831959 inka2-2.4.5/tests/parser/test_is_cloze_note_str.py
+-rw-r--r--   0        0        0      187 2024-02-24 09:57:31.256941 inka2-2.4.5/tests/resources/anki_data/README.txt
+-rw-r--r--   0        0        0        0 2024-02-24 09:57:17.199383 inka2-2.4.5/tests/resources/anki_data/anki.log
+-rw-r--r--   0        0        0    12288 2024-02-24 12:38:03.251271 inka2-2.4.5/tests/resources/anki_data/prefs21.db
+-rw-r--r--   0        0        0      235 2024-02-25 17:01:31.224559 inka2-2.4.5/tests/resources/defaults/config_add_filename.ini
+-rw-r--r--   0        0        0      843 2024-05-30 10:15:52.380031 inka2-2.4.5/tests/resources/index_out_of_range.md
+-rw-r--r--   0        0        0      322 2024-02-24 12:40:05.719614 inka2-2.4.5/tests/resources/test_inka_data.md
+-rw-r--r--   0        0        0      209 2024-02-24 11:13:15.265549 inka2-2.4.5/tests/resources/test_inka_data_init.md
+-rw-r--r--   0        0        0     2203 2023-08-04 16:36:52.832225 inka2-2.4.5/tests/test_anki_media.py
+-rw-r--r--   0        0        0     2567 2024-02-25 14:31:45.346757 inka2-2.4.5/tests/test_basic_note.py
+-rw-r--r--   0        0        0      849 2024-03-10 09:17:53.067716 inka2-2.4.5/tests/test_cli.py
+-rw-r--r--   0        0        0     2202 2024-02-25 14:32:33.200106 inka2-2.4.5/tests/test_cloze_note.py
+-rw-r--r--   0        0        0     4651 2024-02-25 16:50:57.796797 inka2-2.4.5/tests/test_config.py
+-rw-r--r--   0        0        0    14246 2024-02-25 17:25:12.679899 inka2-2.4.5/tests/test_converter.py
+-rw-r--r--   0        0        0     3106 2024-02-24 13:13:12.907154 inka2-2.4.5/tests/test_hasher.py
+-rw-r--r--   0        0        0     1986 2024-02-25 14:34:40.980287 inka2-2.4.5/tests/test_helpers.py
+-rw-r--r--   0        0        0     9929 2024-02-24 13:13:12.805258 inka2-2.4.5/tests/test_highlight.py
+-rw-r--r--   0        0        0     8190 2024-02-24 13:13:12.888067 inka2-2.4.5/tests/test_img_handler.py
+-rw-r--r--   0        0        0      794 2024-02-24 13:13:12.840246 inka2-2.4.5/tests/test_note.py
+-rw-r--r--   0        0        0    21422 2024-03-09 17:27:58.455989 inka2-2.4.5/tests/test_writer.py
+-rw-r--r--   0        0        0     5836 1970-01-01 00:00:00.000000 inka2-2.4.5/PKG-INFO
```

### Comparing `inka2-2.4.4/LICENSE` & `inka2-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/README.md` & `inka2-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/pyproject.toml` & `inka2-2.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "inka2"
-version = "2.4.4"
+version = "2.4.5"
 description = "Command-line tool for adding flashcards from Markdown files to Anki"
 readme = "README.md"
 authors = [
     { name = "sysid", email = "sysid@gmx.de" },
     { name = "Kirill Salnikov", email = "salnikov.k54@gmail.com" },
 ]
 classifiers = [
@@ -79,15 +79,15 @@
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 fail_under = 60
 
 [tool.bumpversion]
-current_version = "2.4.4"
+current_version = "2.4.5"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = [
     "{major}.{minor}.{patch}",
 ]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
```

### Comparing `inka2-2.4.4/src/inka2/cli.py` & `inka2-2.4.5/src/inka2/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,22 +571,27 @@
     initial_directory = os.getcwd()
     for file in files:
         try:
             if update_ids:
                 update_note_ids_in_file(file, anki_api, anki_media)
                 continue
 
-            create_notes_from_file(file, full_sync, anki_api, anki_media, hasher, force=force)
+            create_notes_from_file(
+                file, full_sync, anki_api, anki_media, hasher, force=force
+            )
         except (
             OSError,
             ValueError,
             FileNotFoundError,
             FileExistsError,
         ) as e:
-            print_error(f"{e}\nSkipping file! Consider re-running with --force.", pause=(not ignore_errors))
+            print_error(
+                f"{e}\nSkipping file! Consider re-running with --force.",
+                pause=(not ignore_errors),
+            )
         except AnkiApiError as e:
             print_error(f"{e}\nSkipping file!", pause=(not ignore_errors), note=e.note)
         finally:
             os.chdir(initial_directory)
 
     # Sync changes with AnkiWeb
     print_action("Synchronizing changes with AnkiWeb...")
```

### Comparing `inka2-2.4.4/src/inka2/helpers.py` & `inka2-2.4.5/src/inka2/helpers.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/mistune_plugins/mathjax.py` & `inka2-2.4.5/src/inka2/mistune_plugins/mathjax.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/anki_api.py` & `inka2-2.4.5/src/inka2/models/anki_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import anki
 import anki.collection
 import anki.consts
 import anki.errors
 import anki.models
 import anki.notes
-import aqt
+from aqt.profiles import ProfileManager
 
 from ..exceptions import AnkiApiError
 from .config import Config
 from .notes.note import Note
 
 
 class AnkiApi:
@@ -26,15 +26,15 @@
 
         # Check correctness of the anki path
         meta_path = os.path.join(anki_path, "prefs21.db")
         if not os.path.exists(meta_path):
             raise AnkiApiError(f'incorrect path to Anki folder: "{anki_path}"')
 
         # Initialize profile manager to get access to profile and database actions
-        self._profile_manager = aqt.ProfileManager(anki_path)
+        self._profile_manager = ProfileManager(anki_path)
         self._profile_manager.setupMeta()
 
     def get_profiles(self) -> List[str]:
         """Get list of user profiles from Anki"""
         return self._profile_manager.profiles()
 
     def load_collection(self, profile: str) -> None:
@@ -59,19 +59,22 @@
     def sync(self):
         """Sync collection to AnkiWeb"""
         # todo: handle case when to sync we need user decision (download or upload)
         auth = self._profile_manager.sync_auth()
         if auth is None:
             raise AnkiApiError("Isn't authenticated with AnkiWeb")
 
-        self._collection.save(trx=False)
+        # self._collection.save(trx=False)
 
         # Perform main sync
         try:
-            self._collection.sync_collection(auth)
+            # TODO it throws a warning that it is being running in the main thread
+            # https://forums.ankiweb.net/t/unable-to-sync-login-via-anki-python-pkg-to-ankiweb/43092/4
+            sync_media = self._profile_manager.media_syncing_enabled()
+            self._collection.sync_collection(auth, sync_media)
         except anki.errors.NetworkError:
             raise AnkiApiError("Please check your internet connection")
 
         # Perform media sync
         initial_dir = os.getcwd()
         os.chdir(self._collection.media.dir())
         self._collection.sync_media(auth)
@@ -95,24 +98,24 @@
         return anki_note.id
 
     def update_note_ids(self, notes: Iterable[Note]) -> None:
         """Update incorrect or absent IDs of notes"""
         for note in notes:
             # Update id only if note with this id doesn't exist
             try:
-                note_id = anki.collection.NoteId(note.anki_id if note.anki_id else -1)
+                note_id = anki.notes.NoteId(note.anki_id if note.anki_id else -1)
                 self._collection.get_note(note_id)
             except anki.errors.NotFoundError:
                 found_notes = self._collection.find_notes(note.search_query)
                 note.anki_id = found_notes[0] if found_notes else None
 
     def update_note(self, note: Note) -> None:
         """Synchronize changes in notes with Anki"""
         try:
-            note_id = anki.collection.NoteId(note.anki_id if note.anki_id else -1)
+            note_id = anki.notes.NoteId(note.anki_id if note.anki_id else -1)
             anki_note = self._collection.get_note(note_id)
         except anki.errors.NotFoundError:
             raise AnkiApiError(
                 f"note with ID {note.anki_id} was not found. "
                 f'You can update IDs on notes with the command "inka collect --update-ids path/to/file.md".'
             )
```

### Comparing `inka2-2.4.4/src/inka2/models/anki_media.py` & `inka2-2.4.5/src/inka2/models/anki_media.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/config.py` & `inka2-2.4.5/src/inka2/models/config.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/converter.py` & `inka2-2.4.5/src/inka2/models/converter.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/hasher.py` & `inka2-2.4.5/src/inka2/models/hasher.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/highlighter.py` & `inka2-2.4.5/src/inka2/models/highlighter.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/img_handler.py` & `inka2-2.4.5/src/inka2/models/img_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from typing import Dict, Iterable, List, Optional
 
 from .anki_media import AnkiMedia
 from .notes.note import Note
 
 
 def handle_images_in(
-    notes: List[Note], anki_media: AnkiMedia, copy_images: bool = True, force: bool = False
+    notes: List[Note],
+    anki_media: AnkiMedia,
+    copy_images: bool = True,
+    force: bool = False,
 ) -> None:
     """
     Copy images used in Notes fields to Anki Media folder and change source in their
     links to be just filename (for Anki to find them).
 
     Args:
         notes: Notes in which image links will be searched for and then updated
@@ -70,15 +73,17 @@
 
         for note in notes:
             # We use *updated* fields for replace func cause
             # we need to preserve previous replacements if there are multiple of them
             note.update_fields_with(lambda field: str.replace(field, link, new_link))
 
 
-def _copy_images_to(anki_media: AnkiMedia, image_links: Iterable[str], force: bool = False) -> None:
+def _copy_images_to(
+    anki_media: AnkiMedia, image_links: Iterable[str], force: bool = False
+) -> None:
     """Copy images to Anki Media folder.
 
     Args:
         anki_media: AnkiMedia object that will be used to copy images
         image_links: list of markdown links to images
     Raises:
         FileNotFoundError: if path to image in markdown link is incorrect
```

### Comparing `inka2-2.4.4/src/inka2/models/notes/basic_note.py` & `inka2-2.4.5/src/inka2/models/notes/basic_note.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/notes/cloze_note.py` & `inka2-2.4.5/src/inka2/models/notes/cloze_note.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/notes/note.py` & `inka2-2.4.5/src/inka2/models/notes/note.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/parser.py` & `inka2-2.4.5/src/inka2/models/parser.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/src/inka2/models/writer.py` & `inka2-2.4.5/src/inka2/models/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from pathlib import Path
-from typing import Iterable, Optional, Union, List
+from typing import Iterable, List, Optional, Union
 
+from ..helpers import print_sub_warning
 from .notes.basic_note import BasicNote
 from .notes.cloze_note import ClozeNote
 from .notes.note import Note
 from .parser import Parser
-from ..helpers import print_sub_warning
 
 
 class Writer:
     """Class for editing file with notes"""
 
     def __init__(self, file_path: Union[str, Path], notes: Iterable[Note]):
         self._file_path = file_path
@@ -24,18 +24,22 @@
         """Update lines with IDs of the notes from the file"""
         for note in self._notes:
             # Find note's question in file string
             note_question = note.get_raw_question_field()
 
             all_occurrences = self.find_all_occurrences(note_question)
             if len(all_occurrences) > 1:
-                print_sub_warning(f"Warning: more than one occurrence of '{note_question}' found in {self._file_path}")
+                print_sub_warning(
+                    f"Warning: more than one occurrence of '{note_question}' found in {self._file_path}"
+                )
                 print_sub_warning("Can cause undefined behavior. Please fix.")
 
-            question_string_start = self._file_content.find(note_question)  # TODO: make unambiguous
+            question_string_start = self._file_content.find(
+                note_question
+            )  # TODO: make unambiguous
             if question_string_start == -1:
                 continue
 
             matches = re.finditer(
                 r"(<!--ID:\S+-->)?(\n\d+\.\s*)",
                 self._file_content[:question_string_start],
                 re.MULTILINE,
@@ -61,15 +65,15 @@
             newline_index = question_match.start(2)
 
             if existing_id is None:
                 # Add line with ID after newline
                 self._file_content = (
                     self._file_content[: newline_index + 1]
                     + id_string
-                    + self._file_content[newline_index + 1:]
+                    + self._file_content[newline_index + 1 :]
                 )
             else:
                 # Substitute existing ID with the new one
                 self._file_content = self._file_content.replace(
                     f"<!--ID:{existing_id}-->\n", id_string
                 )
```

### Comparing `inka2-2.4.4/tests/conftest.py` & `inka2-2.4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_cleaned_answer.py` & `inka2-2.4.5/tests/parser/test_get_cleaned_answer.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_deck_name.py` & `inka2-2.4.5/tests/parser/test_get_deck_name.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_id.py` & `inka2-2.4.5/tests/parser/test_get_id.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_note_strings.py` & `inka2-2.4.5/tests/parser/test_get_note_strings.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_notes_from_section.py` & `inka2-2.4.5/tests/parser/test_get_notes_from_section.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_question.py` & `inka2-2.4.5/tests/parser/test_get_question.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_sections.py` & `inka2-2.4.5/tests/parser/test_get_sections.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_get_tags.py` & `inka2-2.4.5/tests/parser/test_get_tags.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_is_basic_note_str.py` & `inka2-2.4.5/tests/parser/test_is_basic_note_str.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/parser/test_is_cloze_note_str.py` & `inka2-2.4.5/tests/parser/test_is_cloze_note_str.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/resources/anki_data/prefs21.db` & `inka2-2.4.5/tests/resources/anki_data/prefs21.db`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/resources/index_out_of_range.md` & `inka2-2.4.5/tests/resources/index_out_of_range.md`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_anki_media.py` & `inka2-2.4.5/tests/test_anki_media.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_basic_note.py` & `inka2-2.4.5/tests/test_basic_note.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_cli.py` & `inka2-2.4.5/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import pytest
 from click.testing import CliRunner
 
 from inka2.cli import ROOT_DIR, cli, get_notes_from_file
 
-
 # Collection of manual test cases
 
 
 @pytest.mark.integration
 def test_hello():
     UNDER_TEST = f"{ROOT_DIR}/tests/resources/test_inka_data.md"
     runner = CliRunner()
-    result = runner.invoke(
-        cli, ["collect", "-u", UNDER_TEST]
-    )
+    result = runner.invoke(cli, ["collect", "-u", UNDER_TEST])
     assert result.exit_code == 0
     print(result.output)
     # assert 'Hello, Test!' in result.output
 
 
 def test_duplicate_question_string_should_fail():
     UNDER_TEST = f"{ROOT_DIR}/tests/resources/index_out_of_range.md"
     runner = CliRunner()
-    result = runner.invoke(
-        cli, ["collect", "-u", UNDER_TEST]
-    )
+    result = runner.invoke(cli, ["collect", "-u", UNDER_TEST])
     assert result.exit_code == 1
 
 
 @pytest.mark.integration
 def test_get_notes_from_file():
     notes = get_notes_from_file(f"{ROOT_DIR}/./tests/resources/test_inka_data.md")  # noqa
     _ = None
```

### Comparing `inka2-2.4.4/tests/test_cloze_note.py` & `inka2-2.4.5/tests/test_cloze_note.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_config.py` & `inka2-2.4.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_converter.py` & `inka2-2.4.5/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_hasher.py` & `inka2-2.4.5/tests/test_hasher.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_helpers.py` & `inka2-2.4.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_highlight.py` & `inka2-2.4.5/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_img_handler.py` & `inka2-2.4.5/tests/test_img_handler.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_note.py` & `inka2-2.4.5/tests/test_note.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/tests/test_writer.py` & `inka2-2.4.5/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `inka2-2.4.4/PKG-INFO` & `inka2-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inka2
-Version: 2.4.4
+Version: 2.4.5
 Summary: Command-line tool for adding flashcards from Markdown files to Anki
 Author-Email: sysid <sysid@gmx.de>, Kirill Salnikov <salnikov.k54@gmail.com>
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
```

