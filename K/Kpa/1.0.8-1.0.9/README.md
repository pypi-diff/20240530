# Comparing `tmp/Kpa-1.0.8.tar.gz` & `tmp/Kpa-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Kpa-1.0.8.tar", last modified: Wed Dec 19 04:27:20 2018, max compression
+gzip compressed data, was "dist/Kpa-1.0.9.tar", last modified: Sat Mar 16 04:59:05 2019, max compression
```

## Comparing `Kpa-1.0.8.tar` & `Kpa-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2018-12-19 04:27:20.000000 Kpa-1.0.8/
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2018-12-19 04:27:20.000000 Kpa-1.0.8/Kpa.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)      348 2018-12-19 04:27:20.000000 Kpa-1.0.8/Kpa.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      438 2018-12-19 04:27:20.000000 Kpa-1.0.8/Kpa.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2018-12-19 04:27:20.000000 Kpa-1.0.8/Kpa.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)       47 2018-12-19 04:27:20.000000 Kpa-1.0.8/Kpa.egg-info/entry_points.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2018-12-18 15:30:55.000000 Kpa-1.0.8/Kpa.egg-info/not-zip-safe
--rw-r--r--   0 peter      (501) staff       (20)        4 2018-12-19 04:27:20.000000 Kpa-1.0.8/Kpa.egg-info/top_level.txt
--rw-r--r--   0 peter      (501) staff       (20)      348 2018-12-19 04:27:20.000000 Kpa-1.0.8/PKG-INFO
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2018-12-19 04:27:20.000000 Kpa-1.0.8/kpa/
--rw-r--r--   0 peter      (501) staff       (20)      216 2018-06-04 02:56:16.000000 Kpa-1.0.8/kpa/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     3902 2018-11-07 21:06:09.000000 Kpa-1.0.8/kpa/cache_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     1797 2018-12-18 15:25:05.000000 Kpa-1.0.8/kpa/command_line.py
--rw-r--r--   0 peter      (501) staff       (20)     1689 2018-12-18 15:26:49.000000 Kpa-1.0.8/kpa/func_cache_utils.py
--rw-r--r--   0 peter      (501) staff       (20)      548 2018-12-03 06:04:45.000000 Kpa-1.0.8/kpa/func_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     2175 2018-12-18 15:25:53.000000 Kpa-1.0.8/kpa/html_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     5711 2018-12-18 15:26:16.000000 Kpa-1.0.8/kpa/http_server.py
--rw-r--r--   0 peter      (501) staff       (20)     3224 2018-12-06 21:32:42.000000 Kpa-1.0.8/kpa/http_utils.py
--rw-r--r--   0 peter      (501) staff       (20)      327 2018-06-04 03:26:23.000000 Kpa-1.0.8/kpa/iter_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     5904 2018-12-18 15:37:16.000000 Kpa-1.0.8/kpa/lazy_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     1038 2018-12-06 21:46:52.000000 Kpa-1.0.8/kpa/pip_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     2787 2018-12-18 15:23:33.000000 Kpa-1.0.8/kpa/terminal_utils.py
--rw-r--r--   0 peter      (501) staff       (20)     3504 2018-12-18 15:24:30.000000 Kpa-1.0.8/kpa/unglob.py
--rw-r--r--   0 peter      (501) staff       (20)       18 2018-12-19 04:27:20.000000 Kpa-1.0.8/kpa/version.py
--rw-r--r--   0 peter      (501) staff       (20)      392 2018-12-19 04:27:20.000000 Kpa-1.0.8/setup.cfg
--rwxr-xr-x   0 peter      (501) staff       (20)     3269 2018-12-18 15:34:28.000000 Kpa-1.0.8/setup.py
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-03-16 04:59:05.000000 Kpa-1.0.9/
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-03-16 04:59:05.000000 Kpa-1.0.9/Kpa.egg-info/
+-rw-r--r--   0 peter      (501) staff       (20)      348 2019-03-16 04:59:05.000000 Kpa-1.0.9/Kpa.egg-info/PKG-INFO
+-rw-r--r--   0 peter      (501) staff       (20)      438 2019-03-16 04:59:05.000000 Kpa-1.0.9/Kpa.egg-info/SOURCES.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2019-03-16 04:59:05.000000 Kpa-1.0.9/Kpa.egg-info/dependency_links.txt
+-rw-r--r--   0 peter      (501) staff       (20)       47 2019-03-16 04:59:05.000000 Kpa-1.0.9/Kpa.egg-info/entry_points.txt
+-rw-r--r--   0 peter      (501) staff       (20)        1 2018-12-18 15:30:55.000000 Kpa-1.0.9/Kpa.egg-info/not-zip-safe
+-rw-r--r--   0 peter      (501) staff       (20)        4 2019-03-16 04:59:05.000000 Kpa-1.0.9/Kpa.egg-info/top_level.txt
+-rw-r--r--   0 peter      (501) staff       (20)      348 2019-03-16 04:59:05.000000 Kpa-1.0.9/PKG-INFO
+drwxr-xr-x   0 peter      (501) staff       (20)        0 2019-03-16 04:59:05.000000 Kpa-1.0.9/kpa/
+-rw-r--r--   0 peter      (501) staff       (20)      216 2018-06-04 02:56:16.000000 Kpa-1.0.9/kpa/__init__.py
+-rw-r--r--   0 peter      (501) staff       (20)     3902 2018-11-07 21:06:09.000000 Kpa-1.0.9/kpa/cache_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     2053 2019-03-16 04:16:35.000000 Kpa-1.0.9/kpa/command_line.py
+-rw-r--r--   0 peter      (501) staff       (20)     1689 2018-12-18 15:26:49.000000 Kpa-1.0.9/kpa/func_cache_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)      548 2018-12-03 06:04:45.000000 Kpa-1.0.9/kpa/func_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     2175 2018-12-18 15:25:53.000000 Kpa-1.0.9/kpa/html_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     7267 2019-03-16 04:41:19.000000 Kpa-1.0.9/kpa/http_server.py
+-rw-r--r--   0 peter      (501) staff       (20)     3222 2019-03-16 03:53:02.000000 Kpa-1.0.9/kpa/http_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)      327 2018-06-04 03:26:23.000000 Kpa-1.0.9/kpa/iter_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     5904 2018-12-18 15:37:16.000000 Kpa-1.0.9/kpa/lazy_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     1038 2018-12-06 21:46:52.000000 Kpa-1.0.9/kpa/pip_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     2787 2018-12-18 15:23:33.000000 Kpa-1.0.9/kpa/terminal_utils.py
+-rw-r--r--   0 peter      (501) staff       (20)     3504 2018-12-18 15:24:30.000000 Kpa-1.0.9/kpa/unglob.py
+-rw-r--r--   0 peter      (501) staff       (20)       18 2019-03-16 04:59:04.000000 Kpa-1.0.9/kpa/version.py
+-rw-r--r--   0 peter      (501) staff       (20)      392 2019-03-16 04:59:05.000000 Kpa-1.0.9/setup.cfg
+-rwxr-xr-x   0 peter      (501) staff       (20)     3269 2018-12-18 15:34:28.000000 Kpa-1.0.9/setup.py
```

### Comparing `Kpa-1.0.8/kpa/cache_utils.py` & `Kpa-1.0.9/kpa/cache_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/command_line.py` & `Kpa-1.0.9/kpa/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
         from .http_server import serve, status_code_server
         serve(status_code_server)
 
     elif sys.argv[1:] == ['dir-server']:
         from .http_server import serve, magic_dir_server
         serve(magic_dir_server)
 
+    elif sys.argv[1:] and sys.argv[1] == 'redirect-server':
+        from .http_server import serve, make_redirect_server
+        port = int(sys.argv[2])
+        target_base_url = sys.argv[3]
+        serve(make_redirect_server(target_base_url), port=port)
+
     elif sys.argv[1:] == ['termcolor']:
         from .terminal_utils import termcolor
         def r(num): return '#' if num is None else str(num%10)
         print('    # ' + ' '.join('{bg:2}'.format(bg=bg) for bg in range(50)))
         for fg in [None]+list(range(0,25)):
             print('{fg if fg is not None else "#":<2} '.format(fg=fg) +
                   ' '.join(termcolor(r(fg)+r(bg), fg, bg) for bg in [None]+list(range(50))))
```

### Comparing `Kpa-1.0.8/kpa/func_cache_utils.py` & `Kpa-1.0.9/kpa/func_cache_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/func_utils.py` & `Kpa-1.0.9/kpa/func_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/html_utils.py` & `Kpa-1.0.9/kpa/html_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/http_server.py` & `Kpa-1.0.9/kpa/http_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 
-import sys, html, urllib
+import sys, html, urllib, re, os
 
 
 def status_code_server(environ, start_response):
     # TODO: query all status codes using [urllib.request.urlopen, requests.get, requests.get.raise_for_status] to compare error-handling
     #  - results should be: (urlopen / requests.get*)
     #    - can't connect => URLError / requests.exceptions.ConnectionError
     #    - 000-100 => BadStatusLine / requests.exceptions.ConnectionError
     #    - 101-199 => HTTPError / ok
     #    - 200-299 => ok
     #    - 301-303,307 with valid "Location:" header => respond for new location
     #    - 300-399 otherwise => HTTPError / ok
     #    - 400-599 => HTTPError / ok (but raise_for_status raises requests.exceptions.HTTPError)
     #    - 600-999 => HTTPError / ok
-    import re
     headers = [('Content-type', 'text/plain')]
     path = environ.get('PATH_INFO','')
 
     m = re.match(r'^/([0-9]{3})/([0-9]{3})$', path)
     if m:
         status = m.group(1) + ' WAT'
         headers.append(('Location', '/{}'.format(m.group(2))))
@@ -29,26 +28,61 @@
         status = m.group(1) + ' WAT'
         ret = 'following xxx path for {}\n'.format(path)
         start_response(status, headers); return [ret.encode('utf8')]
 
     raise Exception('bad url: {path}'.format(**locals()))
 
 
+def make_redirect_server(target_base_url):
+    assert re.match(r'https?://(?:[-a-z0-9]+\.)+[-a-z0-9]+(?:/.*)?', target_base_url)
+    def redirect_server(environ, start_response):
+        headers = [('Content-type', 'text/plain')]
+        path = environ.get('PATH_INFO','')
+        if re.match(r'^[-/a-zA-Z0-9%\.+~_=:]*$', path):
+            status = '302 Found'
+            headers.append(('Location', '{}{}'.format(target_base_url, path)))
+            ret = 'redirecting to {}{}\n'.format(target_base_url, path)
+        else:
+            status = '404 Not Found'
+            ret = 'URL not permitted\n'
+        start_response(status, headers); return [ret.encode('utf8')]
+    return redirect_server
+
+def directory_server(environ, start_response):
+    # TODO: just implement a simple version by hand
+    def normalize_path(path):
+        # This code is taken from http.server.SimpleHTTPRequestHandler.translate_path()
+        import urllib.parse, posixpath
+        path = path.split('?', 1)[0]
+        path = path.split('#', 1)[0]
+        path = urllib.parse.unquote(path)
+        path = posixpath.normpath(path)
+        words = [word for word in path.split('/') if word]
+        path = os.getcwd()
+        for word in words:
+            if os.path.dirname(word) or word in (os.curdir, os.pardir):
+                # ignore components like `.`, `..`, (and also somehow directories?)
+                continue
+            path = os.path.join(path, word)
+        return path
+    path = normalize_path(environ.get('PATH_INFO', ''))
+    
+
+
 def magic_directory_server(environ, start_response):
     # This is like `python3 -m http.server` (http.server.SimpleHTTPRequestHandler).
     # `SimpleHTTPRequestHandler` chooses mimetype using file extension (mimetypes.types_map)
     # This server instead uses mime-guessing
     # I have a solid implementation in `MimeSniffingHTTPRequestHandler` but I'm not sure how to convert it to WSGI/gunicorn
     #    It extends `http.server.SimpleHTTPRequestHandler`
     #       which extends `http.server.BaseHTTPRequestHandler`
     #           which extends `socketserver.StreamRequestHandler`.
     #    It's run using `http.server.test(HandlerClass=MimeSniffingHTTPRequestHandler, ServerClass=http.server.HTTPServer)`
     #       which uses `http.server.HTTPServer(('localhost', 8001), MimeSniffingHTTPRequestHandler).serve_forever()`
     #          which extends `socketserver.TCPServer`
-    import os
     def normalize_path(path):
         # This code is taken from http.server.SimpleHTTPRequestHandler.translate_path()
         import urllib.parse, posixpath
         path = path.split('?', 1)[0]
         path = path.split('#', 1)[0]
         has_trailing_slash = path.rstrip().endswith('/')
         path = urllib.parse.unquote(path)
@@ -114,13 +148,13 @@
     ctype = guess_content_type(path)
     try:
         f = open(path, 'rb')
     except OSError:
         start_response('404 NOTFOUND', [('Connection', 'close')])
     # Note: work-in-progress
 
-def serve(app):
+def serve(app, port=5000):
     from .http_utils import run_gunicorn
     try:
-        run_gunicorn(app)
+        run_gunicorn(app, port=port, use_reloader=False)
     except KeyboardInterrupt:
         pass
```

### Comparing `Kpa-1.0.8/kpa/http_utils.py` & `Kpa-1.0.9/kpa/http_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             if b.open(url):
                 return True
         except Exception:
             pass
     return False
 
 
-def run_gunicorn(app, host='localhost', port=5000, use_reloader=True, num_workers=4, accesslog='-'):
+def run_gunicorn(app, host='0.0.0.0', port=5000, use_reloader=True, num_workers=4, accesslog='-'):
     '''takes a flask app or perhaps other kinds of wsgi apps'''
     # TODO: figure out how to suppress sigwinch
     import gunicorn.app.base
     class StandaloneGunicornApplication(gunicorn.app.base.BaseApplication):
         # from <http://docs.gunicorn.org/en/stable/custom.html>
         def __init__(self, app, opts=None):
             self.application = app
```

### Comparing `Kpa-1.0.8/kpa/lazy_utils.py` & `Kpa-1.0.9/kpa/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/pip_utils.py` & `Kpa-1.0.9/kpa/pip_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/terminal_utils.py` & `Kpa-1.0.9/kpa/terminal_utils.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/kpa/unglob.py` & `Kpa-1.0.9/kpa/unglob.py`

 * *Files identical despite different names*

### Comparing `Kpa-1.0.8/setup.py` & `Kpa-1.0.9/setup.py`

 * *Files identical despite different names*

