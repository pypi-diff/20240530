# Comparing `tmp/platzky-0.2.1.tar.gz` & `tmp/platzky-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platzky-0.2.1.tar", max compression
+gzip compressed data, was "platzky-0.2.2.tar", max compression
```

## Comparing `platzky-0.2.1.tar` & `platzky-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      768 2024-05-28 13:50:00.673695 platzky-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/blog/__init__.py
--rw-r--r--   0        0        0     3031 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/blog/blog.py
--rw-r--r--   0        0        0      513 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/blog/comment_form.py
--rw-r--r--   0        0        0     2203 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/config.py
--rw-r--r--   0        0        0        0 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/__init__.py
--rw-r--r--   0        0        0     2660 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/db.py
--rw-r--r--   0        0        0      905 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/db_loader.py
--rw-r--r--   0        0        0     1513 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/google_json_db.py
--rw-r--r--   0        0        0     6111 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/graph_ql_db.py
--rw-r--r--   0        0        0     3184 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/json_db.py
--rw-r--r--   0        0        0     1010 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/db/json_file_db.py
--rw-r--r--   0        0        0     1450 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/models.py
--rw-r--r--   0        0        0     4649 2024-05-28 13:50:00.673695 platzky-0.2.1/platzky/platzky.py
--rw-r--r--   0        0        0     1106 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/plugin_loader.py
--rw-r--r--   0        0        0     1565 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/plugins/redirections/entrypoint.py
--rw-r--r--   0        0        0     1237 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/plugins/sendmail/entrypoint.py
--rw-r--r--   0        0        0     2710 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/seo/seo.py
--rw-r--r--   0        0        0     7895 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/static/blog.css
--rw-r--r--   0        0        0       78 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/404.html
--rw-r--r--   0        0        0     4966 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/base.html
--rw-r--r--   0        0        0     1281 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/blog.html
--rw-r--r--   0        0        0      526 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/body_meta.html
--rw-r--r--   0        0        0      863 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/feed.xml
--rw-r--r--   0        0        0     1370 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/head_meta.html
--rw-r--r--   0        0        0     3900 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/home.html
--rw-r--r--   0        0        0      647 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/page.html
--rw-r--r--   0        0        0     1906 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/post.html
--rw-r--r--   0        0        0      116 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/robots.txt
--rw-r--r--   0        0        0      578 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/templates/sitemap.xml
--rw-r--r--   0        0        0      725 2024-05-28 13:50:00.677695 platzky-0.2.1/platzky/www_handler.py
--rw-r--r--   0        0        0      841 2024-05-28 13:50:00.677695 platzky-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 platzky-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      768 2024-05-29 23:37:06.179973 platzky-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/blog/__init__.py
+-rw-r--r--   0        0        0     3031 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/blog/blog.py
+-rw-r--r--   0        0        0      513 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/blog/comment_form.py
+-rw-r--r--   0        0        0     2203 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/config.py
+-rw-r--r--   0        0        0        0 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/__init__.py
+-rw-r--r--   0        0        0     2660 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/db.py
+-rw-r--r--   0        0        0      905 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/db_loader.py
+-rw-r--r--   0        0        0     1513 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/google_json_db.py
+-rw-r--r--   0        0        0     6444 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/graph_ql_db.py
+-rw-r--r--   0        0        0     3184 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/json_db.py
+-rw-r--r--   0        0        0     1010 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/db/json_file_db.py
+-rw-r--r--   0        0        0     1450 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/models.py
+-rw-r--r--   0        0        0     4649 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/platzky.py
+-rw-r--r--   0        0        0     1106 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/plugin_loader.py
+-rw-r--r--   0        0        0     1565 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/plugins/redirections/entrypoint.py
+-rw-r--r--   0        0        0     1237 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/plugins/sendmail/entrypoint.py
+-rw-r--r--   0        0        0     2710 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/seo/seo.py
+-rw-r--r--   0        0        0     7895 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/static/blog.css
+-rw-r--r--   0        0        0       78 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/404.html
+-rw-r--r--   0        0        0     4966 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/base.html
+-rw-r--r--   0        0        0     1281 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/blog.html
+-rw-r--r--   0        0        0      526 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/body_meta.html
+-rw-r--r--   0        0        0      863 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/feed.xml
+-rw-r--r--   0        0        0     1370 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/head_meta.html
+-rw-r--r--   0        0        0     3900 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/home.html
+-rw-r--r--   0        0        0      647 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/page.html
+-rw-r--r--   0        0        0     1906 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/post.html
+-rw-r--r--   0        0        0      116 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/robots.txt
+-rw-r--r--   0        0        0      578 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/templates/sitemap.xml
+-rw-r--r--   0        0        0      725 2024-05-29 23:37:06.179973 platzky-0.2.2/platzky/www_handler.py
+-rw-r--r--   0        0        0      841 2024-05-29 23:37:06.179973 platzky-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 platzky-0.2.2/PKG-INFO
```

### Comparing `platzky-0.2.1/README.md` & `platzky-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/blog/blog.py` & `platzky-0.2.2/platzky/blog/blog.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/blog/comment_form.py` & `platzky-0.2.2/platzky/blog/comment_form.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/config.py` & `platzky-0.2.2/platzky/config.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/db/db.py` & `platzky-0.2.2/platzky/db/db.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/db/db_loader.py` & `platzky-0.2.2/platzky/db/db_loader.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/db/google_json_db.py` & `platzky-0.2.2/platzky/db/google_json_db.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/db/graph_ql_db.py` & `platzky-0.2.2/platzky/db/graph_ql_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,22 +22,32 @@
     return GraphQL(config.endpoint, config.token)
 
 
 def db_from_config(config: GraphQlDbConfig):
     return GraphQL(config.endpoint, config.token)
 
 
-def _standarize_post(post):
+def _standarize_comment(
+    comment,
+):  # TODO add tests for checking stadarization of comments
+    return {
+        "author": comment["author"],
+        "comment": comment["comment"],
+        "date": comment["createdAt"],
+    }
+
+
+def _standarize_post(post):  # TODO add tests for checking stadarization of posts
     return {
         "author": post["author"]["name"],
         "slug": post["slug"],
         "title": post["title"],
         "excerpt": post["excerpt"],
         "contentInMarkdown": post["contentInRichText"]["html"],
-        "comments": post["comments"],
+        "comments": [_standarize_comment(comment) for comment in post["comments"]],
         "tags": post["tags"],
         "language": post["language"],
         "coverImage": {
             "url": post["coverImage"]["image"]["url"],
         },
         "date": post["date"],
     }
```

### Comparing `platzky-0.2.1/platzky/db/json_db.py` & `platzky-0.2.2/platzky/db/json_db.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/db/json_file_db.py` & `platzky-0.2.2/platzky/db/json_file_db.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/models.py` & `platzky-0.2.2/platzky/models.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/platzky.py` & `platzky-0.2.2/platzky/platzky.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/plugin_loader.py` & `platzky-0.2.2/platzky/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/plugins/redirections/entrypoint.py` & `platzky-0.2.2/platzky/plugins/redirections/entrypoint.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/plugins/sendmail/entrypoint.py` & `platzky-0.2.2/platzky/plugins/sendmail/entrypoint.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/seo/seo.py` & `platzky-0.2.2/platzky/seo/seo.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/static/blog.css` & `platzky-0.2.2/platzky/static/blog.css`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/base.html` & `platzky-0.2.2/platzky/templates/base.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/blog.html` & `platzky-0.2.2/platzky/templates/blog.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/body_meta.html` & `platzky-0.2.2/platzky/templates/body_meta.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/feed.xml` & `platzky-0.2.2/platzky/templates/feed.xml`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/head_meta.html` & `platzky-0.2.2/platzky/templates/head_meta.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/home.html` & `platzky-0.2.2/platzky/templates/home.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/page.html` & `platzky-0.2.2/platzky/templates/page.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/post.html` & `platzky-0.2.2/platzky/templates/post.html`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/templates/sitemap.xml` & `platzky-0.2.2/platzky/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/platzky/www_handler.py` & `platzky-0.2.2/platzky/www_handler.py`

 * *Files identical despite different names*

### Comparing `platzky-0.2.1/pyproject.toml` & `platzky-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "platzky"
-version = "0.2.1"
+version = "0.2.2"
 description = "Not only blog engine"
 authors = []
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `platzky-0.2.1/PKG-INFO` & `platzky-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platzky
-Version: 0.2.1
+Version: 0.2.2
 Summary: Not only blog engine
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

