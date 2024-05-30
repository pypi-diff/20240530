# Comparing `tmp/proximityhash-1.0.1.tar.gz` & `tmp/proximityhash-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/proximityhash-1.0.1.tar", last modified: Fri Jun 16 09:37:00 2017, max compression
+gzip compressed data, was "proximityhash-3.0.0.tar", last modified: Thu May 30 10:10:56 2024, max compression
```

## Comparing `proximityhash-1.0.1.tar` & `proximityhash-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 Ashwin     (501) staff       (20)        0 2017-06-16 09:37:00.000000 proximityhash-1.0.1/
--rw-r--r--   0 Ashwin     (501) staff       (20)     5111 2017-06-16 09:37:00.000000 proximityhash-1.0.1/PKG-INFO
-drwxr-xr-x   0 Ashwin     (501) staff       (20)        0 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/
--rw-r--r--   0 Ashwin     (501) staff       (20)        1 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/dependency_links.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)       56 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/entry_points.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)     5111 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/PKG-INFO
--rw-r--r--   0 Ashwin     (501) staff       (20)       40 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/requires.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)      297 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/SOURCES.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)       14 2017-06-16 09:37:00.000000 proximityhash-1.0.1/proximityhash.egg-info/top_level.txt
--rw-r--r--   0 Ashwin     (501) staff       (20)     4521 2017-06-16 09:31:54.000000 proximityhash-1.0.1/proximityhash.py
--rw-r--r--   0 Ashwin     (501) staff       (20)     3533 2017-06-16 09:32:03.000000 proximityhash-1.0.1/README.rst
--rw-r--r--   0 Ashwin     (501) staff       (20)      101 2017-06-16 09:37:00.000000 proximityhash-1.0.1/setup.cfg
--rw-r--r--   0 Ashwin     (501) staff       (20)     1075 2017-06-16 09:32:16.000000 proximityhash-1.0.1/setup.py
-drwxr-xr-x   0 Ashwin     (501) staff       (20)        0 2017-06-16 09:37:00.000000 proximityhash-1.0.1/test/
--rw-r--r--   0 Ashwin     (501) staff       (20)     1471 2017-06-07 18:03:45.000000 proximityhash-1.0.1/test/test_proximityhash.py
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2024-05-30 10:10:56.219534 proximityhash-3.0.0/
+-rw-r--r--   0 ashwin     (501) staff       (20)    11389 2024-05-30 09:35:43.000000 proximityhash-3.0.0/LICENSE
+-rw-r--r--   0 ashwin     (501) staff       (20)     4227 2024-05-30 10:10:56.219490 proximityhash-3.0.0/PKG-INFO
+-rw-r--r--   0 ashwin     (501) staff       (20)     3382 2024-05-30 09:31:54.000000 proximityhash-3.0.0/README.rst
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2024-05-30 10:10:56.219297 proximityhash-3.0.0/proximityhash.egg-info/
+-rw-r--r--   0 ashwin     (501) staff       (20)     4227 2024-05-30 10:10:56.000000 proximityhash-3.0.0/proximityhash.egg-info/PKG-INFO
+-rw-r--r--   0 ashwin     (501) staff       (20)      305 2024-05-30 10:10:56.000000 proximityhash-3.0.0/proximityhash.egg-info/SOURCES.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)        1 2024-05-30 10:10:56.000000 proximityhash-3.0.0/proximityhash.egg-info/dependency_links.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       53 2024-05-30 10:10:56.000000 proximityhash-3.0.0/proximityhash.egg-info/entry_points.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       40 2024-05-30 10:10:56.000000 proximityhash-3.0.0/proximityhash.egg-info/requires.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)       14 2024-05-30 10:10:56.000000 proximityhash-3.0.0/proximityhash.egg-info/top_level.txt
+-rw-r--r--   0 ashwin     (501) staff       (20)     5061 2024-04-08 10:54:46.000000 proximityhash-3.0.0/proximityhash.py
+-rw-r--r--   0 ashwin     (501) staff       (20)       80 2024-05-30 10:10:56.219689 proximityhash-3.0.0/setup.cfg
+-rw-r--r--   0 ashwin     (501) staff       (20)     1075 2024-05-30 10:10:52.000000 proximityhash-3.0.0/setup.py
+drwxr-xr-x   0 ashwin     (501) staff       (20)        0 2024-05-30 10:10:56.219011 proximityhash-3.0.0/test/
+-rw-r--r--   0 ashwin     (501) staff       (20)     1471 2023-12-01 16:15:47.000000 proximityhash-3.0.0/test/test_proximityhash.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `proximityhash-1.0.1/proximityhash.py` & `proximityhash-3.0.0/proximityhash.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,39 +49,50 @@
     geohashes = []
 
     grid_width = [5009400.0, 1252300.0, 156500.0, 39100.0, 4900.0, 1200.0, 152.9, 38.2, 4.8, 1.2, 0.149, 0.0370]
     grid_height = [4992600.0, 624100.0, 156000.0, 19500.0, 4900.0, 609.4, 152.4, 19.0, 4.8, 0.595, 0.149, 0.0199]
 
     height = (grid_height[precision - 1])/2
     width = (grid_width[precision-1])/2
+    
+    if (latitude > 60 or latitude < -60):
+        height = (grid_height[precision - 1])/8
+        width = (grid_width[precision-1])/8
+   
+    if (latitude > 82 or latitude < -82):
+        height = (grid_height[precision - 1])/32
+        width = (grid_width[precision-1])/32
+    
+    if (latitude > 89 or latitude < -89):
+        height = (grid_height[precision - 1])/256
+        width = (grid_width[precision-1])/256
 
     lat_moves = int(math.ceil(radius / height)) #4
     lon_moves = int(math.ceil(radius / width)) #2
-
+    
     for i in range(0, lat_moves):
 
         temp_lat = y + height*i
 
         for j in range(0,lon_moves):
-
+           
             temp_lon = x + width*j
-
+            
             if in_circle_check(temp_lat, temp_lon, y, x, radius):
-
                 x_cen, y_cen = get_centroid(temp_lat, temp_lon, height, width)
-
                 lat, lon = convert_to_latlon(y_cen, x_cen, latitude, longitude)
                 points += [[lat, lon]]
                 lat, lon = convert_to_latlon(-y_cen, x_cen, latitude, longitude)
                 points += [[lat, lon]]
                 lat, lon = convert_to_latlon(y_cen, -x_cen, latitude, longitude)
                 points += [[lat, lon]]
                 lat, lon = convert_to_latlon(-y_cen, -x_cen, latitude, longitude)
                 points += [[lat, lon]]
-
+                
+    #print("Points: "+ str(points))
 
     for point in points:
         geohashes += [Geohash.encode(point[0], point[1], precision)]
 
     if georaptor_flag:
         georaptor_out = georaptor.compress(set(geohashes), int(minlevel), int(maxlevel))
         return ','.join(georaptor_out)
@@ -140,8 +151,12 @@
     puts('\n')
     puts(colored.red('Output:'))
 
     print(create_geohash(float(latitude), float(longitude), float(radius), int(precision_level), georaptor_flag, int(minlevel), int(maxlevel)))
 
     et = time.time() - start_time
 
-    puts(colored.green('\nTotal execution time: ' + str(et) + ' seconds\n'))
+    puts(colored.green('\nTotal execution time: ' + str(et) + ' seconds\n'))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `proximityhash-1.0.1/README.rst` & `proximityhash-3.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-.. image:: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b.svg
-   :target: http://donatecoins.org/btc/1HeMeMU2qUFDRZpRQMJ2v27Dw3h3gShJ5b
-
 ProximityHash: Geohashes in Proximity (with the option of compression using Georaptor_)
 =======================================================================================
 
 .. _GeoRaptor: https://github.com/ashwin711/georaptor
 
 Geohash is a geocoding system invented by Gustavo Niemeyer and placed into the public domain. It is a hierarchical
 spatial data structure which subdivides space into buckets of grid shape, which is one of the many applications of
@@ -97,8 +94,8 @@
    limitations under the License.
 
 
 Contributors:
 -------------
 
 - Ashwin Nair [https://github.com/ashwin711]
-- Arjun Menon - [http://github.com/arjunmenon92]
+- Arjun Menon - [http://github.com/arjunmenon92]
```

### Comparing `proximityhash-1.0.1/setup.py` & `proximityhash-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from distutils.core import setup
 import setuptools
 
 setup(
   name = 'proximityhash',
   py_modules = ['proximityhash'],
-  version = '1.0.1',
+  version = '3.0.0',
   description = 'Geohashes in proximity',
   long_description = open('README.rst').read(),
   author = 'Ashwin Nair',
   author_email = 'ashwinnair.ua@gmail.com',
   license = "MIT",
   url = 'https://github.com/ashwin711/proximityhash',
-  download_url = 'https://github.com/ashwin711/proximityhash/tarball/1.0.1',
+  download_url = 'https://github.com/ashwin711/proximityhash/tarball/3.0.0',
   keywords = ['geohash', 'optimizer', 'compression', 'geo', 'latitude', 'longitude', 'coordinates', 'proximity', 'circle'],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Utilities'
   ],
   install_requires = [
 	'clint',
 	'argparse',
-    'georaptor>=2.0.3',
+    'georaptor>=3.0.0',
     'Geohash'
   ],
   entry_points='''
 	[console_scripts]
 	proximityhash=proximityhash:main
   '''
 )
```

### Comparing `proximityhash-1.0.1/test/test_proximityhash.py` & `proximityhash-3.0.0/test/test_proximityhash.py`

 * *Files identical despite different names*

