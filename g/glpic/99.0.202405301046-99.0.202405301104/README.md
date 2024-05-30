# Comparing `tmp/glpic-99.0.202405301046.tar.gz` & `tmp/glpic-99.0.202405301104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405301046.tar", last modified: Thu May 30 10:46:42 2024, max compression
+gzip compressed data, was "glpic-99.0.202405301104.tar", last modified: Thu May 30 11:04:23 2024, max compression
```

## Comparing `glpic-99.0.202405301046.tar` & `glpic-99.0.202405301104.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:46:42.366148 glpic-99.0.202405301046/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 10:46:42.366148 glpic-99.0.202405301046/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-30 10:46:24.000000 glpic-99.0.202405301046/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:46:42.366148 glpic-99.0.202405301046/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-30 10:46:24.000000 glpic-99.0.202405301046/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-30 10:46:24.000000 glpic-99.0.202405301046/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:46:42.366148 glpic-99.0.202405301046/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 10:46:42.000000 glpic-99.0.202405301046/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:46:42.366148 glpic-99.0.202405301046/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-30 10:46:41.000000 glpic-99.0.202405301046/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:04:23.212844 glpic-99.0.202405301104/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 11:04:23.212844 glpic-99.0.202405301104/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-30 11:04:10.000000 glpic-99.0.202405301104/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:04:23.208844 glpic-99.0.202405301104/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-30 11:04:10.000000 glpic-99.0.202405301104/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-30 11:04:10.000000 glpic-99.0.202405301104/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:04:23.212844 glpic-99.0.202405301104/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 11:04:23.000000 glpic-99.0.202405301104/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:04:23.212844 glpic-99.0.202405301104/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-30 11:04:22.000000 glpic-99.0.202405301104/setup.py
```

### Comparing `glpic-99.0.202405301046/README.md` & `glpic-99.0.202405301104/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405301046/glpic/__init__.py` & `glpic-99.0.202405301104/glpic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,18 +168,20 @@
         computers = _get(url, headers=self.headers)
         return computers['data'] if 'data' in computers else []
 
     def info_reservation(self, reservation):
         return _get(f'{self.base_url}/ReservationItem/{reservation}', headers=self.headers)
 
     def list_reservations(self, overrides={}):
+        now = datetime.now()
         user = overrides.get('user') or self.user
         response = _get(f'{self.base_url}/Reservation', headers=self.headers)
         user_id = self.get_user(user)['id']
-        return [r for r in response if r['users_id'] == user_id]
+        l = [r for r in response if r['users_id'] == user_id and datetime.strptime(r['end'], '%Y-%m-%d 00:00:00') > now]
+        return l
 
     def list_computers(self, user=None, overrides={}):
         computers = _get(f'{self.base_url}/search/Computer?uid_cols', headers=self.headers)['data']
         if not overrides:
             return computers
         results = []
         memory = overrides.get('memory')
```

### Comparing `glpic-99.0.202405301046/glpic/cli.py` & `glpic-99.0.202405301104/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405301046/setup.py` & `glpic-99.0.202405301104/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405301046',
+    version='99.0.202405301104',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

