# Comparing `tmp/anipy_cli-3.1.1.tar.gz` & `tmp/anipy_cli-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-3.1.1.tar", max compression
+gzip compressed data, was "anipy_cli-3.1.2.tar", max compression
```

## Comparing `anipy_cli-3.1.1.tar` & `anipy_cli-3.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2308 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/README.md
--rw-r--r--   0        0        0      855 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/arg_parser.py
--rw-r--r--   0        0        0     1922 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/cli.py
--rw-r--r--   0        0        0      411 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/__init__.py
--rw-r--r--   0        0        0      817 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/base_cli.py
--rw-r--r--   0        0        0     2281 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/binge_cli.py
--rw-r--r--   0        0        0     2806 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/default_cli.py
--rw-r--r--   0        0        0     3187 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/download_cli.py
--rw-r--r--   0        0        0     2666 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/history_cli.py
--rw-r--r--   0        0        0     2258 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/mal_cli.py
--rw-r--r--   0        0        0      616 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/seasonal_cli.py
--rw-r--r--   0        0        0      916 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/colors.py
--rw-r--r--   0        0        0    15422 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/config.py
--rw-r--r--   0        0        0     1160 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/discord.py
--rw-r--r--   0        0        0     6981 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/mal_proxy.py
--rw-r--r--   0        0        0      185 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/base_menu.py
--rw-r--r--   0        0        0    24105 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/mal_menu.py
--rw-r--r--   0        0        0     6772 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/menu.py
--rw-r--r--   0        0        0     9097 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/seasonal_menu.py
--rw-r--r--   0        0        0     7229 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/prompts.py
--rw-r--r--   0        0        0     7684 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/util.py
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2308 2024-05-30 12:07:29.289708 anipy_cli-3.1.2/README.md
+-rw-r--r--   0        0        0      855 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5288 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      817 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2806 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3187 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2863 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2258 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15422 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1160 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24105 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     7860 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     7564 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7684 2024-05-30 12:07:29.293708 anipy_cli-3.1.2/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.2/PKG-INFO
```

### Comparing `anipy_cli-3.1.1/README.md` & `anipy_cli-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/pyproject.toml` & `anipy_cli-3.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-cli"
-version = "3.1.1"
+version = "3.1.2"
 description = "Watch and Download anime from the comfort of your Terminal"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-cli"
 keywords = ["anime", "cli"]
@@ -16,15 +16,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 yaspin = "^3.0.2"
 inquirerpy = "^0.3.4"
 appdirs = "^1.4.4"
 pypresence = "^4.3.0"
-anipy-api = "^3.1.1"
+anipy-api = "^3.1.2"
 
 [tool.poetry.scripts]
 anipy-cli = "anipy_cli.cli:run_cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sdaqo/anipy-cli/issues"
```

### Comparing `anipy_cli-3.1.1/src/anipy_cli/arg_parser.py` & `anipy_cli-3.1.2/src/anipy_cli/arg_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Union
 
 from anipy_cli import __version__
 
 
-@dataclass(frozen=True)
+@dataclass()
 class CliArgs:
     download: bool
     binge: bool
     history: bool
     seasonal: bool
     mal: bool
     delete: bool
```

### Comparing `anipy_cli-3.1.1/src/anipy_cli/cli.py` & `anipy_cli-3.1.2/src/anipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/base_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/base_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/binge_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/default_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/default_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/download_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/download_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/history_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/history_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import TYPE_CHECKING, Optional
 
+from InquirerPy.base.control import Choice
 from anipy_api.anime import Anime
 from anipy_api.locallist import LocalList, LocalListEntry
 from InquirerPy import inquirer
 
 from anipy_cli.clis.base_cli import CliBase
 from anipy_cli.colors import colors
 from anipy_cli.config import Config
@@ -38,24 +39,27 @@
 
         if not history:
             print("You have no History, exiting")
             return False
 
         entry = inquirer.fuzzy(  # type: ignore
             message="Select History Entry:",
-            choices=history,
+            choices=[
+                Choice(value=h, name=f"{n + 1}. {repr(h)}")
+                for n, h in enumerate(history)
+            ],
             long_instruction="To cancel this prompt press ctrl+z",
             mandatory=False,
         ).execute()
 
         if entry is None:
             return False
 
-        self.history_entry = entry
-        self.anime = Anime.from_local_list_entry(entry)
+        self.history_entry = LocalListEntry.from_dict(entry)
+        self.anime = Anime.from_local_list_entry(self.history_entry)
 
     def process(self):
         assert self.anime is not None
         assert self.history_entry is not None
 
         with DotSpinner(
             "Extracting streams for ",
```

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/mal_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/mal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/clis/seasonal_cli.py` & `anipy_cli-3.1.2/src/anipy_cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/colors.py` & `anipy_cli-3.1.2/src/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/config.py` & `anipy_cli-3.1.2/src/anipy_cli/config.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/discord.py` & `anipy_cli-3.1.2/src/anipy_cli/discord.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/mal_proxy.py` & `anipy_cli-3.1.2/src/anipy_cli/mal_proxy.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/menus/base_menu.py` & `anipy_cli-3.1.2/src/anipy_cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/menus/mal_menu.py` & `anipy_cli-3.1.2/src/anipy_cli/menus/mal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/menus/menu.py` & `anipy_cli-3.1.2/src/anipy_cli/menus/menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import sys
 from typing import TYPE_CHECKING, List
 
+from InquirerPy import inquirer
+from InquirerPy.base.control import Choice
 from anipy_api.download import Downloader
-from anipy_api.provider import LanguageTypeEnum
+from anipy_api.provider import LanguageTypeEnum, ProviderStream
 from anipy_api.locallist import LocalList
 
 from anipy_cli.colors import colors, cprint
 from anipy_cli.config import Config
 from anipy_cli.menus.base_menu import MenuBase, MenuOption
 from anipy_cli.util import DotSpinner, error, get_download_path, migrate_locallist
 from anipy_cli.prompts import pick_episode_prompt, search_show_prompt
 
 
 if TYPE_CHECKING:
     from anipy_api.anime import Anime
     from anipy_api.player import PlayerBase
-    from anipy_api.provider import Episode, ProviderStream
+    from anipy_api.provider import Episode
 
     from anipy_cli.arg_parser import CliArgs
 
 
 class Menu(MenuBase):
     def __init__(
         self,
@@ -49,14 +51,15 @@
                 self.change_type,
                 "c",
             ),
             MenuOption("Select episode", self.selec_ep, "s"),
             MenuOption("Select from history", self.selec_hist, "h"),
             MenuOption("Search for Anime", self.search, "a"),
             MenuOption("Add to seasonals", self.add_seasonal, "t"),
+            MenuOption("Change video quality", self.change_quality, "v"),
             MenuOption("Print Video Info", self.video_info, "i"),
             MenuOption("Download Episode", self.download_video, "d"),
             MenuOption("Quit", self.quit, "q"),
         ]
 
     def print_header(self):
         cprint(
@@ -164,14 +167,44 @@
 
     def add_seasonal(self):
         self.seasonal_list.update(
             self.anime, episode=self.stream.episode, language=self.stream.language
         )
         cprint(colors.GREEN, "Anime added to seasonals!")
 
+    def change_quality(self):
+        with DotSpinner(
+            "Extracting streams for ",
+            colors.BLUE,
+            f"{self.anime.name} ({self.lang})",
+            " Episode ",
+            self.stream.episode,
+            "...",
+        ):
+            streams = self.anime.get_videos(self.stream.episode, self.lang)
+            streams.reverse()
+
+        stream = inquirer.select(  # type: ignore
+            message="Select Stream:",
+            choices=[
+                Choice(value=s, name=f"{s.resolution}p - {s.url}") for s in streams
+            ],
+            long_instruction="To skip this prompt press ctrl+z",
+            mandatory=False,
+        ).execute()
+
+        if stream is None:
+            return
+
+        stream = ProviderStream(**stream)
+        self.options.quality = stream.resolution
+        self.stream = stream
+        self.player.play_title(self.anime, self.stream)
+        self.print_options()
+
     def download_video(self):
         config = Config()
         with DotSpinner("Starting Download...") as s:
 
             def progress_indicator(percentage: float):
                 s.set_text(f"Downloading ({percentage:.1f}%)")
```

### Comparing `anipy_cli-3.1.1/src/anipy_cli/menus/seasonal_menu.py` & `anipy_cli-3.1.2/src/anipy_cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/src/anipy_cli/prompts.py` & `anipy_cli-3.1.2/src/anipy_cli/prompts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from typing import TYPE_CHECKING, Optional, List, Tuple
 from InquirerPy import inquirer
+from InquirerPy.base.control import Choice
 from anipy_api.provider import (
     BaseProvider,
     FilterCapabilities,
     Filters,
     LanguageTypeEnum,
     Season,
 )
@@ -68,15 +69,17 @@
     if len(results) == 0:
         error("no search results")
         # Do not prompt for season again
         return search_show_prompt(mode, skip_season_search=True)
 
     anime = inquirer.fuzzy(  # type: ignore
         message="Select Show:",
-        choices=results,
+        choices=[
+            Choice(value=r, name=f"{n + 1}. {repr(r)}") for n, r in enumerate(results)
+        ],
         long_instruction=(
             "\nS = Anime is available in sub\n"
             "D = Anime is available in dub\n"
             "First two letters indicate the provider\n"
             "To skip this prompt press ctrl+z"
         ),
         mandatory=False,
@@ -114,16 +117,23 @@
     results = [
         Anime.from_search_result(provider, r)
         for r in provider.get_search(query="", filters=filters)
     ]
 
     anime = inquirer.fuzzy(  # type: ignore
         message="Select Show:",
-        choices=results,
-        long_instruction="\nS = Anime is available in sub\nD = Anime is available in dub\nTo skip this prompt press ctrl+z",
+        choices=[
+            Choice(value=r, name=f"{n + 1}. {repr(r)}") for n, r in enumerate(results)
+        ],
+        long_instruction=(
+            "\nS = Anime is available in sub\n"
+            "D = Anime is available in dub\n"
+            "First two letters indicate the provider\n"
+            "To skip this prompt press ctrl+z"
+        ),
         mandatory=False,
     ).execute()
 
     return anime
 
 
 def pick_episode_prompt(
```

### Comparing `anipy_cli-3.1.1/src/anipy_cli/util.py` & `anipy_cli-3.1.2/src/anipy_cli/util.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.1/PKG-INFO` & `anipy_cli-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 3.1.1
+Version: 3.1.2
 Summary: Watch and Download anime from the comfort of your Terminal
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anipy-api (>=3.1.1,<4.0.0)
+Requires-Dist: anipy-api (>=3.1.2,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pypresence (>=4.3.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: yaspin (>=3.0.2,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/sdaqo/anipy-cli/issues
 Project-URL: Documentation, https://sdaqo.github.io/anipy-cli/getting-started-cli
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.1 Summary: Watch and
+Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.2 Summary: Watch and
 Download anime from the comfort of your Terminal Home-page: https://
 sdaqo.github.io/anipy-cli License: GPL-3.0 Keywords: anime,cli Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: anipy-api (>=3.1.1,<4.0.0) Requires-Dist: appdirs
+Python :: 3.12 Requires-Dist: anipy-api (>=3.1.2,<4.0.0) Requires-Dist: appdirs
 (>=1.4.4,<2.0.0) Requires-Dist: inquirerpy (>=0.3.4,<0.4.0) Requires-Dist:
 pypresence (>=4.3.0,<5.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
 Dist: yaspin (>=3.0.2,<4.0.0) Project-URL: Bug Tracker, https://github.com/
 sdaqo/anipy-cli/issues Project-URL: Documentation, https://sdaqo.github.io/
 anipy-cli/getting-started-cli Project-URL: Repository, https://github.com/
 sdaqo/anipy-cli Description-Content-Type: text/markdown # ANIPY-CLI **Anime
 from the comfort of your Terminal**
```

