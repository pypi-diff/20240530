# Comparing `tmp/voyger-0.2.tar.gz` & `tmp/voyger-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyger-0.2.tar", last modified: Thu May 30 15:00:35 2024, max compression
+gzip compressed data, was "voyger-0.3.5.tar", last modified: Thu May 30 16:14:38 2024, max compression
```

## Comparing `voyger-0.2.tar` & `voyger-0.3.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 15:00:35.754701 voyger-0.2/
--rw-rw-rw-   0        0        0      170 2024-05-30 15:00:35.750385 voyger-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-30 15:00:35.754701 voyger-0.2/setup.cfg
--rw-rw-rw-   0        0        0      327 2024-05-30 14:43:30.000000 voyger-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:00:35.748384 voyger-0.2/voyger.egg-info/
--rw-rw-rw-   0        0        0      170 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 15:00:35.000000 voyger-0.2/voyger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      565 2024-05-30 14:59:34.000000 voyger-0.2/voyger.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:14:38.118248 voyger-0.3.5/
+-rw-rw-rw-   0        0        0      172 2024-05-30 16:14:38.115247 voyger-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:14:38.118248 voyger-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      329 2024-05-30 16:13:47.000000 voyger-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:14:38.113249 voyger-0.3.5/voyger.egg-info/
+-rw-rw-rw-   0        0        0      172 2024-05-30 16:14:37.000000 voyger-0.3.5/voyger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-05-30 16:14:37.000000 voyger-0.3.5/voyger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:14:37.000000 voyger-0.3.5/voyger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 16:14:37.000000 voyger-0.3.5/voyger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      628 2024-05-30 16:13:21.000000 voyger-0.3.5/voyger.py
```

### Comparing `voyger-0.2/voyger.py` & `voyger-0.3.5/voyger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # voyger.py
 
 class rocket():
-    def __init__(self, name :str, mass : int, velocity : int, thrust : int):
+    def __init__(self, name :str, mass : int, velocity : int, thrust : int, show_static = False):
         self.name : str = name
         self.mass : int = mass 
         self.velocity : int = velocity
         self.thrust : int = thrust
-        
-    def rocket_state(rocket : any):
-        print("Name : ",rocket.name)
-        print("Mass : ",rocket.mass)
-        print("Velocity : ",rocket.velocity)
-        print("Thrust : ",rocket.thrust)
+        if show_static is not False:
+            print("Name : ",rocket.name)
+            print("Mass : ",rocket.mass)
+            print("Velocity : ",rocket.velocity)
+            print("Thrust : ",rocket.thrust)
+            print("Show_Static : ",rocket.show_static)
+    
         
         
 voyger = rocket("voyger", 1000, 800, 30)
-rocket.rocket_state(voyger)
+
```

