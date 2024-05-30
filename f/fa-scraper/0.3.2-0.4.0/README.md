# Comparing `tmp/fa-scraper-0.3.2.tar.gz` & `tmp/fa_scraper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-scraper-0.3.2.tar", max compression
+gzip compressed data, was "fa_scraper-0.4.0.tar", max compression
```

## Comparing `fa-scraper-0.3.2.tar` & `fa_scraper-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/LICENSE
--rw-r--r--   0        0        0     1796 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/README.md
--rw-r--r--   0        0        0      269 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/fa_scraper/__init__.py
--rw-r--r--   0        0        0     2346 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/fa_scraper/cli.py
--rwxr-xr-x   0        0        0     6905 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/fa_scraper/fa_scraper.py
--rw-r--r--   0        0        0      551 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/fa_scraper/types.py
--rw-r--r--   0        0        0     1141 2022-04-30 23:17:47.808739 fa-scraper-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2790 2022-04-30 23:17:54.275504 fa-scraper-0.3.2/setup.py
--rw-r--r--   0        0        0     3207 2022-04-30 23:17:54.275919 fa-scraper-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-04-30 22:55:43.964040 fa_scraper-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1796 2022-04-30 22:55:43.964040 fa_scraper-0.4.0/README.md
+-rw-r--r--   0        0        0      269 2024-05-30 21:16:29.595151 fa_scraper-0.4.0/fa_scraper/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-30 20:28:12.981408 fa_scraper-0.4.0/fa_scraper/cli.py
+-rwxr-xr-x   0        0        0     9412 2024-05-30 20:28:12.981408 fa_scraper-0.4.0/fa_scraper/fa_scraper.py
+-rw-r--r--   0        0        0      654 2024-05-30 20:28:12.981408 fa_scraper-0.4.0/fa_scraper/types.py
+-rw-r--r--   0        0        0     1149 2024-05-30 20:43:05.864810 fa_scraper-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 fa_scraper-0.4.0/PKG-INFO
```

### Comparing `fa-scraper-0.3.2/LICENSE` & `fa_scraper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fa-scraper-0.3.2/README.md` & `fa_scraper-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fa-scraper-0.3.2/fa_scraper/cli.py` & `fa_scraper-0.4.0/fa_scraper/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     )
     parser.add_argument("--all-lists", action="store_true", help="download all lists")
     parser.add_argument(
         "--version", action="version", version="%(prog)s {}".format(__version__)
     )
     parser.add_argument(
         "--ignore",
-        help="ignore category (default: all)",
+        help="ignore category (default: none)",
         type=FACategory,
         choices=FACategory,
         action="append",
         default=[],
     )
 
     args = parser.parse_args()
```

### Comparing `fa-scraper-0.3.2/fa_scraper/fa_scraper.py` & `fa_scraper-0.4.0/fa_scraper/fa_scraper.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import csv
 from typing import Any, Iterable, Iterator, List, Mapping, Sequence
 
 import arrow
 import bs4
 import requests
 
-from .types import FACategory, FAList, Lang, ListId, UserId
+from .types import FACategory, FAList, Lang, ListId, UserId, Page
 
 # FilmAffinity root URL
 FA_ROOT_URL = "https://www.filmaffinity.com/{lang}/"
 
 FILM_FIELDNAMES = (
     "Title",
     "Year",
@@ -37,14 +37,31 @@
 
 LIST_FIELDNAMES = (
     "Title",
     "Year",
     "Directors",
 )
 
+SKIP_BY_LANG = {
+    Lang.ES: {
+        FACategory.TVS: "Serie",
+        FACategory.TVMS: "Miniserie",
+        FACategory.TV: "TV",
+    },
+    Lang.EN: {
+        FACategory.TVS: "tv series",
+        FACategory.TVMS: "miniseries",
+        FACategory.TV: "TV",
+    },
+}
+
+TITLE_ERROR_TEMPLATE = "Unexpected error while parsing data for title '{title}'"
+PAGE_ERROR_TEMPLATE = "Unexpected error while parsing data on page '{page}'"
+SKIP_TITLE_TEMPLATE = "Skipping {title} since it is a '{title_type}'"
+
 
 def get_date(tag: bs4.element.Tag, lang: Lang) -> str:
     """Gets date from tag (format YYYY-MM-DD)"""
 
     if not tag.string:
         raise ValueError("Missing date on tag {}".format(tag))
 
@@ -75,52 +92,36 @@
 
     return ", ".join(
         sanitize_director_tag(d)
         for d in tag.find_all(class_="mc-director")[0].find_all(class_="nb")
     )
 
 
-def is_chosen_category(
-    tag: bs4.element.Tag, lang: Lang, ignore_list: Iterable[FACategory]
+def should_skip_type(
+    title_type: str, lang: Lang, ignore_list: Iterable[FACategory]
 ) -> bool:
-    """Checks if given tag is within the chosen categories"""
-
-    title = tag.find_all(class_="mc-title")[0].a.string.strip()
-
-    if lang == Lang.ES:
-        skipdct = {
-            FACategory.TVS: "(Serie de TV)",
-            FACategory.TVMS: "(Miniserie de TV)",
-            FACategory.TV: "(TV)",
-            FACategory.S: "(C)",
-        }
-    else:
-        skipdct = {
-            FACategory.TVS: "(TV Series)",
-            FACategory.TVMS: "(TV Miniseries)",
-            FACategory.TV: "(TV)",
-            FACategory.S: "(S)",
-        }
+    """Checks if given title type should be skipped."""
+    for category in ignore_list:
+        if title_type == SKIP_BY_LANG[lang][category]:
+            return True
+    return False
 
-    skip = map(skipdct.get, ignore_list)
 
-    return not any(title.endswith(suffix) for suffix in skip)
-
-
-def pages_from(template: str) -> Iterator[bs4.BeautifulSoup]:
+def pages_from(template: str) -> Iterator[Page]:
     """Yields pages from a given section until one of them fails."""
 
     eof = False
     n = 1
 
     while not eof:
-        request = requests.get(template.format(n))
+        url = template.format(n)
+        request = requests.get(url)
         request.encoding = "utf-8"
 
-        yield bs4.BeautifulSoup(request.text, "lxml")
+        yield Page(url=url, contents=bs4.BeautifulSoup(request.text, "lxml"))
 
         eof = request.status_code != 200
         if not eof:
             print("Page {n}".format(n=n), end="\r")
         else:
             print("Page {n}. Download complete!".format(n=n - 1))
         n += 1
@@ -132,70 +133,130 @@
     """Yields films rated by user given user id"""
 
     FA = (FA_ROOT_URL + "userratings.php?user_id={id}&p={{}}&orderby=4").format(
         lang=lang, id=user_id
     )
 
     for page in pages_from(FA):
-        tags = page.find_all(class_=["user-ratings-header", "user-ratings-movie"])
-        cur_date = None
-
-        for tag in tags:
-            if tag["class"] == ["user-ratings-header"]:
-                cur_date = get_date(tag, lang)
-            elif is_chosen_category(tag, lang, ignore_list):
-                title = tag.find_all(class_="mc-title")[0].a
-                yield {
-                    "Title": title.string.strip(),
-                    "Year": title.next_sibling.strip()[1:-1],
-                    "Directors": get_directors(tag),
-                    "WatchedDate": cur_date,
-                    "Rating": int(tag.find_all(class_="ur-mr-rat")[0].string) / 2,
-                    "Rating10": tag.find_all(class_="ur-mr-rat")[0].string,
-                }
+        try:
+            tags = page.contents.find_all(
+                class_=["user-ratings-header", "user-ratings-movie"]
+            )
+            cur_date = None
+
+            for tag in tags:
+                if tag["class"] == ["user-ratings-header"]:
+                    cur_date = get_date(tag, lang)
+                else:
+                    try:
+                        title = tag.find_all(class_="mc-title")[0].a
+                        title_name = title.string.strip()
+                        title_type = tag.find_all(class_="d-flex")[0].find_all(
+                            class_="type"
+                        )
+                        if title_type and should_skip_type(
+                            title_type[0].string.strip(), lang, ignore_list
+                        ):
+                            print(
+                                SKIP_TITLE_TEMPLATE.format(
+                                    title=title_name,
+                                    title_type=title_type[0].string.strip(),
+                                )
+                            )
+                            continue
+
+                        yield {
+                            "Title": title.string.strip(),
+                            "Year": int(
+                                tag.find_all(class_="d-flex")[0]
+                                .find_all(class_="mc-year")[0]
+                                .string.strip()
+                            ),
+                            "Directors": get_directors(tag),
+                            "WatchedDate": cur_date,
+                            "Rating": int(tag.find_all(class_="ur-mr-rat")[0].string)
+                            / 2,
+                            "Rating10": tag.find_all(class_="ur-mr-rat")[0].string,
+                        }
+                    except:
+                        print(TITLE_ERROR_TEMPLATE.format(title=title.string.strip()))
+                        raise
+        except:
+            print(PAGE_ERROR_TEMPLATE.format(page=page.url))
+            raise
 
 
 def get_list_data(
     user_id: UserId, list_id: ListId, lang: Lang, ignore_list: Iterable[FACategory]
-) -> Iterator[Mapping[str, str]]:
+) -> Iterator[Mapping[str, Any]]:
     """Yields films from list given list id"""
 
     FA = (
         FA_ROOT_URL + "userlist.php?user_id={user_id}&list_id={list_id}&page={{}}"
     ).format(lang=lang, user_id=user_id, list_id=list_id)
 
     for page in pages_from(FA):
-        tags = page.find_all(class_=["movie-wrapper"])
+        try:
+            tags = page.contents.find_all(class_=["movie-wrapper"])
 
-        for tag in tags:
-            if is_chosen_category(tag, lang, ignore_list):
-                title = tag.find_all(class_="mc-title")[0].a
-                yield {
-                    "Title": title.string.strip(),
-                    "Year": title.next_sibling.strip()[1:-1],
-                    "Directors": get_directors(tag),
-                }
+            for tag in tags:
+                try:
+                    title = tag.find_all(class_="mc-title")[0].a
+                    title_name = title.string.strip()
+                    title_type = tag.find_all(class_="d-flex")[0].find_all(
+                        class_="type"
+                    )
+                    if title_type and should_skip_type(
+                        title_type[0].string.strip(), lang, ignore_list
+                    ):
+                        print(
+                            SKIP_TITLE_TEMPLATE.format(
+                                title=title_name,
+                                title_type=title_type[0].string.strip(),
+                            )
+                        )
+                        continue
+
+                    yield {
+                        "Title": title_name,
+                        "Year": int(
+                            tag.find_all(class_="d-flex")[0]
+                            .find_all(class_="mc-year")[0]
+                            .string.strip()
+                        ),
+                        "Directors": get_directors(tag),
+                    }
+                except:
+                    print(TITLE_ERROR_TEMPLATE.format(title=title_name))
+                    raise
+        except:
+            print(PAGE_ERROR_TEMPLATE.format(page=page.url))
+            raise
 
 
 def get_user_lists(user_id: UserId, lang: Lang) -> Iterator[FAList]:
     """Yields all lists from the given user"""
 
     FA = (FA_ROOT_URL + "userlists.php?user_id={user_id}&p={{}}").format(
         lang=lang, user_id=user_id
     )
 
     for page in pages_from(FA):
-        tags = page.find_all(class_=["list-name-wrapper"])
-        for tag in tags:
-            list_name = tag.text.split("\n")[1]
-            list_name = "".join(w for w in list_name if w.isalnum() or w == " ")
-
-            url = tag.a.get("href")
-            list_id = ListId(url[url.find("list_id=") + len("list_id=") :])
-            yield FAList(list_id, list_name)
+        try:
+            tags = page.contents.find_all(class_=["list-name-wrapper"])
+            for tag in tags:
+                list_name = tag.text.split("\n")[1]
+                list_name = "".join(w for w in list_name if w.isalnum() or w == " ")
+
+                url = tag.a.get("href")
+                list_id = ListId(url[url.find("list_id=") + len("list_id=") :])
+                yield FAList(list_id, list_name)
+        except:
+            print(PAGE_ERROR_TEMPLATE.format(page=page.url))
+            raise
 
 
 def save_lists_to_csv(
     user_id: UserId, lang: Lang, pattern: str, ignore_list: Iterable[FACategory]
 ):
     """Extracts all lists from a user and saves them independently"""
```

### Comparing `fa-scraper-0.3.2/fa_scraper/types.py` & `fa_scraper-0.4.0/fa_scraper/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from enum import Enum
 from typing import NamedTuple, NewType
+from dataclasses import dataclass
+import bs4
 
 
 class FACategory(Enum):
     """FilmAffinity categories"""
 
     TVS = "TVS"
     TVMS = "TVMS"
     TV = "TV"
-    S = "S"
 
     def __str__(self):
         """Returns category"""
         return self.value
 
 
 class Lang(Enum):
@@ -25,7 +26,13 @@
         """Returns option code"""
         return self.value
 
 
 UserId = NewType("UserId", str)
 ListId = NewType("ListId", str)
 FAList = NamedTuple("FAList", [("id", ListId), ("name", str)])
+
+
+@dataclass
+class Page:
+    url: str
+    contents: bs4.BeautifulSoup
```

### Comparing `fa-scraper-0.3.2/pyproject.toml` & `fa_scraper-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fa-scraper"
-version = "0.3.2"
+version = "0.4.0"
 description = "A Letterboxd-compatible FilmAffinity scraper."
 license = "GPL-3.0-or-later"
 authors = ["Pablo Baeyens <pbaeyens31+github@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/mx-psi/fa-scraper"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -21,22 +21,22 @@
 "Authors" = "https://github.com/mx-psi/fa-scraper/blob/master/AUTHORS"
 
 [tool.poetry.scripts]
 fa-scrapper = "fa_scraper.cli:main"
 fa-scraper = "fa_scraper.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.9"
 beautifulsoup4 = "^4.9.1"
 requests = "^2.21.0"
-lxml = "^4.5.1"
+lxml = ">=4.5.1,<6.0.0"
 arrow = "^1.2.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
+pytest = "^8.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `fa-scraper-0.3.2/PKG-INFO` & `fa_scraper-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: fa-scraper
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Letterboxd-compatible FilmAffinity scraper.
 Home-page: https://github.com/mx-psi/fa-scraper
 License: GPL-3.0-or-later
 Author: Pablo Baeyens
 Author-email: pbaeyens31+github@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: arrow (>=1.2.1,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
-Requires-Dist: lxml (>=4.5.1,<5.0.0)
+Requires-Dist: lxml (>=4.5.1,<6.0.0)
 Requires-Dist: requests (>=2.21.0,<3.0.0)
 Project-URL: Authors, https://github.com/mx-psi/fa-scraper/blob/master/AUTHORS
 Project-URL: Bug Tracker, https://github.com/mx-psi/fa-scraper/issues
 Project-URL: Changelog, https://github.com/mx-psi/fa-scraper/blob/master/CHANGELOG.md
 Project-URL: Repository, https://github.com/mx-psi/fa-scraper
 Description-Content-Type: text/markdown
```

