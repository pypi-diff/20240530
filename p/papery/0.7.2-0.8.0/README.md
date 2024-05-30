# Comparing `tmp/papery-0.7.2.tar.gz` & `tmp/papery-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papery-0.7.2.tar", last modified: Sun Jan 21 05:38:18 2024, max compression
+gzip compressed data, was "papery-0.8.0.tar", last modified: Thu May 30 09:26:18 2024, max compression
```

## Comparing `papery-0.7.2.tar` & `papery-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,57 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    11358 2020-10-23 03:53:53.000000 papery-0.7.2/LICENSE
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2409 2024-01-21 05:38:18.175427 papery-0.7.2/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1889 2024-01-19 04:12:09.000000 papery-0.7.2/README.md
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.171428 papery-0.7.2/papery/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      662 2024-01-21 05:36:59.000000 papery-0.7.2/papery/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.167429 papery-0.7.2/papery/data/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery/data/sample/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      251 2024-01-19 04:12:09.000000 papery-0.7.2/papery/data/sample/README.md
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      240 2022-11-23 07:16:00.000000 papery-0.7.2/papery/data/sample/config.yml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery/data/sample/files/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      134 2020-10-23 03:53:53.000000 papery-0.7.2/papery/data/sample/files/robots.txt
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery/data/sample/pages/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1782 2024-01-19 04:12:09.000000 papery-0.7.2/papery/data/sample/pages/index.md
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      253 2024-01-19 04:12:09.000000 papery-0.7.2/papery/data/sample/pages/index.yml
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.171428 papery-0.7.2/papery/data/sample/themes/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.171428 papery-0.7.2/papery/data/sample/themes/default/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.171428 papery-0.7.2/papery/data/sample/themes/default/assets/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery/data/sample/themes/default/assets/css/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1484 2024-01-19 04:12:09.000000 papery-0.7.2/papery/data/sample/themes/default/assets/css/style.css
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery/data/sample/themes/default/templates/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      481 2020-10-23 03:53:53.000000 papery-0.7.2/papery/data/sample/themes/default/templates/base.tmpl
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       97 2020-10-23 03:53:53.000000 papery-0.7.2/papery/data/sample/themes/default/templates/footer.tmpl
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      448 2024-01-19 04:12:09.000000 papery-0.7.2/papery/data/sample/themes/default/templates/page.tmpl
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4047 2024-01-21 05:34:27.000000 papery-0.7.2/papery/engine.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery/lint_configs/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      615 2022-11-02 05:19:18.000000 papery-0.7.2/papery/lint_configs/config_schema.yaml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1391 2022-11-02 05:19:18.000000 papery-0.7.2/papery/lint_configs/markdownlint.yaml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       51 2022-11-02 05:19:18.000000 papery-0.7.2/papery/lint_configs/yamllint.yaml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     9322 2024-01-19 04:12:09.000000 papery-0.7.2/papery/page.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3313 2022-11-02 05:34:12.000000 papery-0.7.2/papery/papery.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    11271 2024-01-19 04:12:09.000000 papery-0.7.2/papery/rendering.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4645 2020-10-23 03:53:53.000000 papery-0.7.2/papery/serving.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1803 2022-11-23 07:16:00.000000 papery-0.7.2/papery/sitemap.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      275 2020-10-23 03:53:53.000000 papery-0.7.2/papery/sitemap_template.xml
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2307 2020-10-23 03:53:53.000000 papery-0.7.2/papery/util.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5162 2024-01-19 04:12:09.000000 papery-0.7.2/papery/validate.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/papery.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2409 2024-01-21 05:38:18.000000 papery-0.7.2/papery.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      892 2024-01-21 05:38:18.000000 papery-0.7.2/papery.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2024-01-21 05:38:18.000000 papery-0.7.2/papery.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       70 2024-01-21 05:38:18.000000 papery-0.7.2/papery.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        7 2024-01-21 05:38:18.000000 papery-0.7.2/papery.egg-info/top_level.txt
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/scripts/
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)      670 2022-11-02 05:19:18.000000 papery-0.7.2/scripts/papery
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2024-01-21 05:38:18.179427 papery-0.7.2/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4689 2022-11-23 07:16:00.000000 papery-0.7.2/setup.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2024-01-21 05:38:18.175427 papery-0.7.2/tests/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      611 2022-11-23 07:16:00.000000 papery-0.7.2/tests/test_sitemap.py
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.446555 papery-0.8.0/
+-rw-r--r--   0 nashida    (501) staff       (20)    11358 2020-12-14 05:55:48.000000 papery-0.8.0/LICENSE
+-rw-r--r--   0 nashida    (501) staff       (20)     2409 2024-05-30 09:26:18.445831 papery-0.8.0/PKG-INFO
+-rw-r--r--   0 nashida    (501) staff       (20)     1889 2024-05-01 09:28:42.000000 papery-0.8.0/README.md
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.442576 papery-0.8.0/papery/
+-rw-r--r--   0 nashida    (501) staff       (20)      662 2024-05-30 08:54:12.000000 papery-0.8.0/papery/__init__.py
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.439753 papery-0.8.0/papery/data/
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.443374 papery-0.8.0/papery/data/sample/
+-rw-r--r--   0 nashida    (501) staff       (20)      251 2023-08-28 04:28:08.000000 papery-0.8.0/papery/data/sample/README.md
+-rw-r--r--   0 nashida    (501) staff       (20)      240 2023-08-23 09:16:33.000000 papery-0.8.0/papery/data/sample/config.yml
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.443494 papery-0.8.0/papery/data/sample/files/
+-rw-r--r--   0 nashida    (501) staff       (20)      134 2020-12-14 05:55:48.000000 papery-0.8.0/papery/data/sample/files/robots.txt
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.444054 papery-0.8.0/papery/data/sample/output/
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.440013 papery-0.8.0/papery/data/sample/output/assets/
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.444179 papery-0.8.0/papery/data/sample/output/assets/css/
+-rw-r--r--   0 nashida    (501) staff       (20)     1484 2023-08-24 09:42:21.000000 papery-0.8.0/papery/data/sample/output/assets/css/style.css
+-rw-r--r--   0 nashida    (501) staff       (20)     9366 2024-05-02 07:59:24.000000 papery-0.8.0/papery/data/sample/output/index.html
+-rw-r--r--   0 nashida    (501) staff       (20)      134 2020-12-14 05:55:48.000000 papery-0.8.0/papery/data/sample/output/robots.txt
+-rw-r--r--   0 nashida    (501) staff       (20)      233 2024-05-02 07:59:24.000000 papery-0.8.0/papery/data/sample/output/sitemap.xml
+-rw-r--r--   0 nashida    (501) staff       (20)      196 2024-05-02 07:59:24.000000 papery-0.8.0/papery/data/sample/output/sitemap.xml.gz
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.444420 papery-0.8.0/papery/data/sample/pages/
+-rw-r--r--   0 nashida    (501) staff       (20)     1951 2024-05-30 08:47:57.000000 papery-0.8.0/papery/data/sample/pages/index.md
+-rw-r--r--   0 nashida    (501) staff       (20)      253 2023-08-28 04:28:08.000000 papery-0.8.0/papery/data/sample/pages/index.yml
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.440190 papery-0.8.0/papery/data/sample/themes/
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.440358 papery-0.8.0/papery/data/sample/themes/default/
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.440294 papery-0.8.0/papery/data/sample/themes/default/assets/
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.444537 papery-0.8.0/papery/data/sample/themes/default/assets/css/
+-rw-r--r--   0 nashida    (501) staff       (20)     1484 2023-08-24 09:42:21.000000 papery-0.8.0/papery/data/sample/themes/default/assets/css/style.css
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.444882 papery-0.8.0/papery/data/sample/themes/default/templates/
+-rw-r--r--   0 nashida    (501) staff       (20)      481 2023-08-30 08:25:58.000000 papery-0.8.0/papery/data/sample/themes/default/templates/base.tmpl
+-rw-r--r--   0 nashida    (501) staff       (20)       97 2020-12-14 05:55:48.000000 papery-0.8.0/papery/data/sample/themes/default/templates/footer.tmpl
+-rw-r--r--   0 nashida    (501) staff       (20)      448 2023-08-28 04:28:08.000000 papery-0.8.0/papery/data/sample/themes/default/templates/page.tmpl
+-rw-r--r--   0 nashida    (501) staff       (20)     4434 2024-05-30 08:47:57.000000 papery-0.8.0/papery/engine.py
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.445217 papery-0.8.0/papery/lint_configs/
+-rw-r--r--   0 nashida    (501) staff       (20)      615 2021-06-08 00:57:49.000000 papery-0.8.0/papery/lint_configs/config_schema.yaml
+-rw-r--r--   0 nashida    (501) staff       (20)     1391 2023-08-31 02:50:45.000000 papery-0.8.0/papery/lint_configs/markdownlint.yaml
+-rw-r--r--   0 nashida    (501) staff       (20)       51 2021-06-08 00:57:49.000000 papery-0.8.0/papery/lint_configs/yamllint.yaml
+-rw-r--r--   0 nashida    (501) staff       (20)     9451 2024-05-30 08:47:57.000000 papery-0.8.0/papery/page.py
+-rw-r--r--   0 nashida    (501) staff       (20)     3549 2024-05-14 08:52:08.000000 papery-0.8.0/papery/papery.py
+-rw-r--r--   0 nashida    (501) staff       (20)    11399 2024-05-14 08:52:08.000000 papery-0.8.0/papery/rendering.py
+-rw-r--r--   0 nashida    (501) staff       (20)     4847 2024-05-14 08:52:08.000000 papery-0.8.0/papery/serving.py
+-rw-r--r--   0 nashida    (501) staff       (20)     1803 2023-01-27 08:24:42.000000 papery-0.8.0/papery/sitemap.py
+-rw-r--r--   0 nashida    (501) staff       (20)      275 2020-12-14 05:55:48.000000 papery-0.8.0/papery/sitemap_template.xml
+-rw-r--r--   0 nashida    (501) staff       (20)     2307 2020-12-14 05:55:48.000000 papery-0.8.0/papery/util.py
+-rw-r--r--   0 nashida    (501) staff       (20)     5162 2023-09-01 04:53:28.000000 papery-0.8.0/papery/validate.py
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.445613 papery-0.8.0/papery.egg-info/
+-rw-r--r--   0 nashida    (501) staff       (20)     2409 2024-05-30 09:26:18.000000 papery-0.8.0/papery.egg-info/PKG-INFO
+-rw-r--r--   0 nashida    (501) staff       (20)     1092 2024-05-30 09:26:18.000000 papery-0.8.0/papery.egg-info/SOURCES.txt
+-rw-r--r--   0 nashida    (501) staff       (20)        1 2024-05-30 09:26:18.000000 papery-0.8.0/papery.egg-info/dependency_links.txt
+-rw-r--r--   0 nashida    (501) staff       (20)       70 2024-05-30 09:26:18.000000 papery-0.8.0/papery.egg-info/requires.txt
+-rw-r--r--   0 nashida    (501) staff       (20)        7 2024-05-30 09:26:18.000000 papery-0.8.0/papery.egg-info/top_level.txt
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.445332 papery-0.8.0/scripts/
+-rwxr-xr-x   0 nashida    (501) staff       (20)      670 2022-08-29 01:33:48.000000 papery-0.8.0/scripts/papery
+-rw-r--r--   0 nashida    (501) staff       (20)       38 2024-05-30 09:26:18.446597 papery-0.8.0/setup.cfg
+-rw-r--r--   0 nashida    (501) staff       (20)     4715 2024-05-30 09:16:17.000000 papery-0.8.0/setup.py
+drwxr-xr-x   0 nashida    (501) staff       (20)        0 2024-05-30 09:26:18.445455 papery-0.8.0/tests/
+-rw-r--r--   0 nashida    (501) staff       (20)      611 2023-01-27 08:24:42.000000 papery-0.8.0/tests/test_sitemap.py
```

### Comparing `papery-0.7.2/LICENSE` & `papery-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/PKG-INFO` & `papery-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papery
-Version: 0.7.2
+Version: 0.8.0
 Summary: A simple static site generator - supports Markdown, YAML and JSON inputs and Jinja2 templating
 Home-page: https://github.com/withletters/papery
 Author: Xcoo, Inc.
 Author-email: developer@xcoo.jp
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `papery-0.7.2/README.md` & `papery-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery/__init__.py` & `papery-0.8.0/papery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from __future__ import absolute_import
 
-version = "0.7.2"
+version = "0.8.0"
```

### Comparing `papery-0.7.2/papery/data/sample/pages/index.md` & `papery-0.8.0/papery/data/sample/pages/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # My web site
 
+[toc]
+
 Welecome to my web site with [papery](http://github.com/withletters/papery)
 
 :smile: :heart: :thumbsup:
 
 ## A Happy Post
 
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
@@ -32,14 +34,25 @@
 def factorial(x):
     if x == 0:
         return 1
     else:
         return x * factorial(x - 1)
 ```
 
+### Code block inside the lists
+
+1. You can add
+
+    ``` text
+    Some code block
+    Inside the lists
+    ```
+
+2. And continue indexing...
+
 ## Permalink
 
 ### Permalink h3
 
 #### Permalink h4
 
 ##### Permalink h5
@@ -87,21 +100,19 @@
 <summary> How to use </summary>
 
 #### Markdown text
 
 - A *Markdown* text
 - Here is a example with `details` element
 
-``` html
-<details markdown="block">
-<summary> Example </summary>
-
-#### Example
-
-Something Markdown text...
-
-</details>
-```
-
+    ``` html
+    <details markdown="block">
+    <summary> Example </summary>
+
+    #### Example
+
+    Some Markdown text...
+    </details>
+    ```
 </details>
 
 ### My Favorite Fruits
```

### Comparing `papery-0.7.2/papery/data/sample/themes/default/assets/css/style.css` & `papery-0.8.0/papery/data/sample/output/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery/engine.py` & `papery-0.8.0/papery/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,20 +58,28 @@
 
         parser_build = subparsers.add_parser('build',
                                              help='build site')
         parser_build.add_argument('--debug',
                                   type=int,
                                   help='output debug log')
 
+        parser_build.add_argument('-s','--skip-validation',
+                                  action='store_true',
+                                  help='build resources without validation')
+
         parser_run = subparsers.add_parser('run',
                                            help='run development server')
         parser_run.add_argument('--debug',
                                 type=int,
                                 help='output debug log')
 
+        parser_run.add_argument('-s','--skip-validation',
+                                action='store_true',
+                                help='run development server without validation')
+
         parser_init = subparsers.add_parser('init',
                                             help='initialize site')
         parser_init.add_argument('--debug',
                                  type=int,
                                  help='output debug log')
 
         parser_clean = subparsers.add_parser('clean',
```

### Comparing `papery-0.7.2/papery/lint_configs/config_schema.yaml` & `papery-0.8.0/papery/lint_configs/config_schema.yaml`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery/lint_configs/markdownlint.yaml` & `papery-0.8.0/papery/lint_configs/markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery/page.py` & `papery-0.8.0/papery/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,27 +54,29 @@
 
         html = markdown.markdown(text,
                                  extensions=["tables",
                                              "fenced_code",
                                              "codehilite",
                                              "pymdownx.emoji",
                                              "md_in_html",
-                                             "toc"],
+                                             "toc",
+                                             "pymdownx.superfences"],
                                  extension_configs={
                                      "codehilite": {
                                          "noclasses": "True"
                                      },
                                      "pymdownx.emoji": {
                                          "emoji_index": pymdownx.emoji.gemoji,
                                          "emoji_generator": pymdownx.emoji.to_png,
                                          "alt": "short",
                                          "options": {
                                              # TODO make "image_path" configurable by papery's configuration file for security reasons
                                          }},
                                      "toc": {
+                                         "marker": "[toc]",
                                          "permalink": "True",
                                          "slugify": markdown.extensions.toc.slugify_unicode
                                      }})
         if link is None:
             return html
         else:
             return self._build_link(html)
```

### Comparing `papery-0.7.2/papery/papery.py` & `papery-0.8.0/papery/papery.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,36 +45,38 @@
             self.favicon_dir = ''
 
     def render(self, **args):
         renderer = papery.rendering.Renderer(self.config,
                                              self.themes_dir,
                                              self.files_dir,
                                              self.favicon_dir,
-                                             self.output_dir)
+                                             self.output_dir,
+                                             args['skip_validation'])
         renderer.run()
 
     def run_server(self, **args):
-        self.render()
+        self.render(skip_validation=args['skip_validation'])
 
         watch_dirs = []
 
         theme_path = os.path.join(self.themes_dir, self.config["theme"])
         watch_dirs.append(os.path.abspath(theme_path))
 
         for page in self.config["pages"]:
             page_dirpath = os.path.dirname(page["file"])
             watch_dirs.append(os.path.abspath(page_dirpath))
 
         server = papery.serving.Server(root_dir=self.output_dir,
                                        watch_dirs=watch_dirs,
-                                       change_handler=self.rebuild)
+                                       change_handler=self.rebuild,
+                                       skip_validation=args['skip_validation'])
         server.run()
 
-    def rebuild(self):
-        self.render()
+    def rebuild(self, **args):
+        self.render(skip_validation=args['skip_validation'])
 
     def clean(self, **args):
         renderer = papery.rendering.Renderer(self.config,
                                              self.themes_dir,
                                              self.files_dir,
                                              self.favicon_dir,
                                              self.output_dir)
```

### Comparing `papery-0.7.2/papery/rendering.py` & `papery-0.8.0/papery/rendering.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,26 @@
 
 class Renderer(object):
 
     def __init__(self, config,
                  themes_dir="themes",
                  files_dir="files",
                  favicon_dir="",
-                 output_dir="output"):
+                 output_dir="output",
+                 skip_validation=False):
         fixed_config = {}
         for k, v in config.items():
             fixed_config[re.sub('-', '_', k)] = v
         self.config = fixed_config
 
         self.output_dir = output_dir
         self.themes_dir = themes_dir
         self.files_dir = files_dir
         self.favicon_dir = favicon_dir
+        self.skip_validation = skip_validation
 
         if "theme" not in self.config:
             self.config["theme"] = "default"
 
         if "pages" not in self.config:
             self.config['pages'] = []
 
@@ -76,15 +78,16 @@
             self.favicon_dir = os.path.join(self.themes_dir, self.config["theme"])
 
         self._targets = {}
         self._page_maps = []
 
     def run(self):
         self._check()
-        self._validate()
+        if not self.skip_validation:
+            self._validate()
         self._prepare_output()
         self._scan()
         self._render_pages()
         self._copy_assets()
         self._generate_sitemap()
 
     def clean(self):
```

### Comparing `papery-0.7.2/papery/serving.py` & `papery-0.8.0/papery/serving.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,29 +32,30 @@
 
 # TODO(takashi) refactor
 
 
 class Server(object):
 
     def __init__(self, root_dir=None, host='', port=8000,
-                 watch_dirs=[], change_handler=None):
+                 watch_dirs=[], change_handler=None, skip_validation=False):
         self.root_dir = os.path.abspath(root_dir)
         self.host = host
         self.port = port
         self.watch_dirs = [os.path.abspath(d) for d in watch_dirs]
         self.change_handler = change_handler
+        self.skip_validation = skip_validation
 
         self.work_dir = os.getcwd()
 
     def run(self):
         if self.root_dir:
             os.chdir(self.root_dir)
 
         wrap = RebuildHandlerWrapper(self.change_handler, self.watch_dirs,
-                                     self.work_dir)
+                                     self.work_dir, self.skip_validation)
         req_handler = wrap.request_handler
 
         HTTPServer.allow_reuse_address = True
 
         server = HTTPServer((self.host, self.port), req_handler)
         socket_info = server.socket.getsockname()
 
@@ -68,22 +69,23 @@
             print("\nStopping development server...")
         finally:
             server.shutdown()
 
 
 class RebuildHandlerWrapper(object):
 
-    def __init__(wrap_self, rebuild, watch_dirs, work_dir):
+    def __init__(wrap_self, rebuild, watch_dirs, work_dir, skip_validation):
         """
         We can't pass arugments to HTTPRequestHandlers, because HTTPServer
         calls __init__. So make a closure.
         """
         wrap_self.rebuild = rebuild
         wrap_self.watch_dirs = watch_dirs
         wrap_self.work_dir = work_dir
+        wrap_self.skip_validation = skip_validation
 
         wrap_self._modtime_sum = None
         wrap_self.changed()
 
         class RebuildHandler(SimpleHTTPRequestHandler):
             """Rebuild if something has changed."""
 
@@ -98,15 +100,15 @@
                 """
                 Handle a request and, if anything has changed, rebuild the
                 site before responding.
                 """
                 if wrap_self.changed():
                     current_dir = os.getcwd()
                     os.chdir(wrap_self.work_dir)
-                    wrap_self.rebuild()
+                    wrap_self.rebuild(skip_validation=wrap_self.skip_validation)
                     os.chdir(current_dir)
 
                 SimpleHTTPRequestHandler.handle(self)
 
         wrap_self.request_handler = RebuildHandler
 
     def _sum_modified_time(self, scan_dirs):
```

### Comparing `papery-0.7.2/papery/sitemap.py` & `papery-0.8.0/papery/sitemap.py`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery/util.py` & `papery-0.8.0/papery/util.py`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery/validate.py` & `papery-0.8.0/papery/validate.py`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/papery.egg-info/PKG-INFO` & `papery-0.8.0/papery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papery
-Version: 0.7.2
+Version: 0.8.0
 Summary: A simple static site generator - supports Markdown, YAML and JSON inputs and Jinja2 templating
 Home-page: https://github.com/withletters/papery
 Author: Xcoo, Inc.
 Author-email: developer@xcoo.jp
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `papery-0.7.2/papery.egg-info/SOURCES.txt` & `papery-0.8.0/papery.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 papery.egg-info/SOURCES.txt
 papery.egg-info/dependency_links.txt
 papery.egg-info/requires.txt
 papery.egg-info/top_level.txt
 papery/data/sample/README.md
 papery/data/sample/config.yml
 papery/data/sample/files/robots.txt
+papery/data/sample/output/index.html
+papery/data/sample/output/robots.txt
+papery/data/sample/output/sitemap.xml
+papery/data/sample/output/sitemap.xml.gz
+papery/data/sample/output/assets/css/style.css
 papery/data/sample/pages/index.md
 papery/data/sample/pages/index.yml
 papery/data/sample/themes/default/assets/css/style.css
 papery/data/sample/themes/default/templates/base.tmpl
 papery/data/sample/themes/default/templates/footer.tmpl
 papery/data/sample/themes/default/templates/page.tmpl
 papery/lint_configs/config_schema.yaml
```

### Comparing `papery-0.7.2/scripts/papery` & `papery-0.8.0/scripts/papery`

 * *Files identical despite different names*

### Comparing `papery-0.7.2/setup.py` & `papery-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from __future__ import print_function
 
-from setuptools import setup, convert_path
+from setuptools import setup
+from distutils.util import convert_path
 from fnmatch import fnmatchcase
 import os
 import sys
 
 from papery import version
 
 standard_exclude = ('*.py', '*.pyc', '*~', '.*', '*.bak')
```

### Comparing `papery-0.7.2/tests/test_sitemap.py` & `papery-0.8.0/tests/test_sitemap.py`

 * *Files identical despite different names*

