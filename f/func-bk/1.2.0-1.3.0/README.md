# Comparing `tmp/func_bk-1.2.0.tar.gz` & `tmp/func_bk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.2.0.tar", last modified: Sat May 18 13:28:55 2024, max compression
+gzip compressed data, was "func_bk-1.3.0.tar", last modified: Thu May 30 12:34:43 2024, max compression
```

## Comparing `func_bk-1.2.0.tar` & `func_bk-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 13:28:55.546787 func_bk-1.2.0/
--rw-rw-rw-   0        0        0     2701 2024-05-18 13:28:55.545787 func_bk-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2484 2024-05-18 13:15:48.000000 func_bk-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 13:28:55.539787 func_bk-1.2.0/func_bk/
--rw-rw-rw-   0        0        0     4121 2024-05-18 13:06:54.000000 func_bk-1.2.0/func_bk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 13:28:55.544788 func_bk-1.2.0/func_bk.egg-info/
--rw-rw-rw-   0        0        0     2701 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-14 13:47:26.000000 func_bk-1.2.0/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-05-18 13:28:55.000000 func_bk-1.2.0/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-05-18 13:28:55.546787 func_bk-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-05-18 13:16:54.000000 func_bk-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:43.040879 func_bk-1.3.0/
+-rw-rw-rw-   0        0        0     2994 2024-05-30 12:34:43.040879 func_bk-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:43.034879 func_bk-1.3.0/func_bk/
+-rw-rw-rw-   0        0        0     2491 2024-05-30 10:23:47.000000 func_bk-1.3.0/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.3.0/func_bk/django.py
+-rw-rw-rw-   0        0        0     4602 2024-05-30 12:25:20.000000 func_bk-1.3.0/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:43.039879 func_bk-1.3.0/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     2994 2024-05-30 12:34:42.000000 func_bk-1.3.0/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-30 12:34:42.000000 func_bk-1.3.0/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:34:42.000000 func_bk-1.3.0/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-30 12:34:42.000000 func_bk-1.3.0/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-05-30 12:34:42.000000 func_bk-1.3.0/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-30 12:34:43.041880 func_bk-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-05-30 12:34:31.000000 func_bk-1.3.0/setup.py
```

### Comparing `func_bk-1.2.0/PKG-INFO` & `func_bk-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.2.0
+Version: 1.3.0
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
@@ -53,15 +53,15 @@
 
 
 call_functions_by_partial_name(partial_name, *args, **kwargs): use all function with partial name
 
 CFBPN=call_functions_by_partial_name
 Fcall=call_functions_by_partial_name
 
-
+DJANGO:
 
 
 function for django:
 
 
 allpath(route: str, view, name: str): It is used to create a list of URL routes that support both the presence and absence of a trailing slash
 
@@ -100,7 +100,15 @@
     class index(LBASE):
         model=Tovar
         template_name="mains/icecream_list.html"
         context_object_name='date'
         paginate_by=5
         paginate_orphans=2
         page_n=5 ...
+
+
+FAST_API:
+
+path(): this is django path for fast api, He have args from FastAPI.get() or FastAPI.post etc, new arguments=
+        app:your app FastAPI
+        func:function from your FastAPI
+        type:str, type:'get','post','put','delete','patch'(register is not important)
```

### Comparing `func_bk-1.2.0/README.md` & `func_bk-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 
 call_functions_by_partial_name(partial_name, *args, **kwargs): use all function with partial name
 
 CFBPN=call_functions_by_partial_name
 Fcall=call_functions_by_partial_name
 
-
+DJANGO:
 
 
 function for django:
 
 
 allpath(route: str, view, name: str): It is used to create a list of URL routes that support both the presence and absence of a trailing slash
 
@@ -92,8 +92,16 @@
     example:
     class index(LBASE):
         model=Tovar
         template_name="mains/icecream_list.html"
         context_object_name='date'
         paginate_by=5
         paginate_orphans=2
-        page_n=5 ...
+        page_n=5 ...
+
+
+FAST_API:
+
+path(): this is django path for fast api, He have args from FastAPI.get() or FastAPI.post etc, new arguments=
+        app:your app FastAPI
+        func:function from your FastAPI
+        type:str, type:'get','post','put','delete','patch'(register is not important)
```

### Comparing `func_bk-1.2.0/func_bk.egg-info/PKG-INFO` & `func_bk-1.3.0/func_bk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.2.0
+Version: 1.3.0
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
@@ -53,15 +53,15 @@
 
 
 call_functions_by_partial_name(partial_name, *args, **kwargs): use all function with partial name
 
 CFBPN=call_functions_by_partial_name
 Fcall=call_functions_by_partial_name
 
-
+DJANGO:
 
 
 function for django:
 
 
 allpath(route: str, view, name: str): It is used to create a list of URL routes that support both the presence and absence of a trailing slash
 
@@ -100,7 +100,15 @@
     class index(LBASE):
         model=Tovar
         template_name="mains/icecream_list.html"
         context_object_name='date'
         paginate_by=5
         paginate_orphans=2
         page_n=5 ...
+
+
+FAST_API:
+
+path(): this is django path for fast api, He have args from FastAPI.get() or FastAPI.post etc, new arguments=
+        app:your app FastAPI
+        func:function from your FastAPI
+        type:str, type:'get','post','put','delete','patch'(register is not important)
```

