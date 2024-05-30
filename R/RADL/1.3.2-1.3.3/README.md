# Comparing `tmp/RADL-1.3.2.tar.gz` & `tmp/RADL-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RADL-1.3.2.tar", last modified: Thu Jan 12 09:42:28 2023, max compression
+gzip compressed data, was "RADL-1.3.3.tar", last modified: Thu May 30 06:19:12 2024, max compression
```

## Comparing `RADL-1.3.2.tar` & `RADL-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-01-12 09:42:28.634037 RADL-1.3.2/
--rw-rw-r--   0 micafer   (1000) micafer   (1000)      791 2022-10-03 09:19:40.000000 RADL-1.3.2/INSTALL
--rw-rw-r--   0 micafer   (1000) micafer   (1000)    35147 2022-10-03 09:19:40.000000 RADL-1.3.2/LICENSE
--rw-rw-r--   0 micafer   (1000) micafer   (1000)       65 2022-10-03 09:19:40.000000 RADL-1.3.2/MANIFEST.in
--rw-rw-r--   0 micafer   (1000) micafer   (1000)     1042 2022-10-03 09:19:40.000000 RADL-1.3.2/NOTICE
--rw-rw-r--   0 micafer   (1000) micafer   (1000)      631 2023-01-12 09:42:28.634037 RADL-1.3.2/PKG-INFO
-drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-01-12 09:42:28.630037 RADL-1.3.2/RADL.egg-info/
--rw-rw-r--   0 micafer   (1000) micafer   (1000)      631 2023-01-12 09:42:28.000000 RADL-1.3.2/RADL.egg-info/PKG-INFO
--rw-rw-r--   0 micafer   (1000) micafer   (1000)      283 2023-01-12 09:42:28.000000 RADL-1.3.2/RADL.egg-info/SOURCES.txt
--rw-rw-r--   0 micafer   (1000) micafer   (1000)        1 2023-01-12 09:42:28.000000 RADL-1.3.2/RADL.egg-info/dependency_links.txt
--rw-rw-r--   0 micafer   (1000) micafer   (1000)        4 2023-01-12 09:42:28.000000 RADL-1.3.2/RADL.egg-info/requires.txt
--rw-rw-r--   0 micafer   (1000) micafer   (1000)        5 2023-01-12 09:42:28.000000 RADL-1.3.2/RADL.egg-info/top_level.txt
--rw-rw-r--   0 micafer   (1000) micafer   (1000)     1832 2022-10-03 09:19:40.000000 RADL-1.3.2/README
--rw-rw-r--   0 micafer   (1000) micafer   (1000)     1375 2023-01-12 09:42:19.000000 RADL-1.3.2/changelog
-drwxrwxr-x   0 micafer   (1000) micafer   (1000)        0 2023-01-12 09:42:28.630037 RADL-1.3.2/radl/
--rw-rw-r--   0 micafer   (1000) micafer   (1000)      804 2023-01-12 09:42:19.000000 RADL-1.3.2/radl/__init__.py
--rw-rw-r--   0 micafer   (1000) micafer   (1000)    13323 2022-10-03 09:20:37.000000 RADL-1.3.2/radl/parsetab.py
--rw-rw-r--   0 micafer   (1000) micafer   (1000)    53485 2023-01-12 09:42:11.000000 RADL-1.3.2/radl/radl.py
--rw-rw-r--   0 micafer   (1000) micafer   (1000)     8633 2023-01-12 09:42:19.000000 RADL-1.3.2/radl/radl_json.py
--rw-rw-r--   0 micafer   (1000) micafer   (1000)    12276 2022-10-03 09:19:40.000000 RADL-1.3.2/radl/radl_parse.py
--rw-rw-r--   0 micafer   (1000) micafer   (1000)       38 2023-01-12 09:42:28.634037 RADL-1.3.2/setup.cfg
--rw-rw-r--   0 micafer   (1000) micafer   (1000)     1614 2022-10-03 09:19:40.000000 RADL-1.3.2/setup.py
+drwxr-xr-x   0 micafer   (1000) micafer   (1000)        0 2024-05-30 06:19:12.215840 RADL-1.3.3/
+-rw-r--r--   0 micafer   (1000) micafer   (1000)      791 2024-05-30 06:05:31.000000 RADL-1.3.3/INSTALL
+-rw-r--r--   0 micafer   (1000) micafer   (1000)    35147 2024-05-30 06:05:31.000000 RADL-1.3.3/LICENSE
+-rw-r--r--   0 micafer   (1000) micafer   (1000)       65 2024-05-30 06:05:31.000000 RADL-1.3.3/MANIFEST.in
+-rw-r--r--   0 micafer   (1000) micafer   (1000)     1042 2024-05-30 06:05:31.000000 RADL-1.3.3/NOTICE
+-rw-r--r--   0 micafer   (1000) micafer   (1000)      631 2024-05-30 06:19:12.215840 RADL-1.3.3/PKG-INFO
+drwxr-xr-x   0 micafer   (1000) micafer   (1000)        0 2024-05-30 06:19:12.215840 RADL-1.3.3/RADL.egg-info/
+-rw-r--r--   0 micafer   (1000) micafer   (1000)      631 2024-05-30 06:19:12.000000 RADL-1.3.3/RADL.egg-info/PKG-INFO
+-rw-r--r--   0 micafer   (1000) micafer   (1000)      266 2024-05-30 06:19:12.000000 RADL-1.3.3/RADL.egg-info/SOURCES.txt
+-rw-r--r--   0 micafer   (1000) micafer   (1000)        1 2024-05-30 06:19:12.000000 RADL-1.3.3/RADL.egg-info/dependency_links.txt
+-rw-r--r--   0 micafer   (1000) micafer   (1000)       14 2024-05-30 06:19:12.000000 RADL-1.3.3/RADL.egg-info/requires.txt
+-rw-r--r--   0 micafer   (1000) micafer   (1000)        5 2024-05-30 06:19:12.000000 RADL-1.3.3/RADL.egg-info/top_level.txt
+-rw-r--r--   0 micafer   (1000) micafer   (1000)     1832 2024-05-30 06:05:31.000000 RADL-1.3.3/README
+-rw-r--r--   0 micafer   (1000) micafer   (1000)     1464 2024-05-30 06:06:05.000000 RADL-1.3.3/changelog
+drwxr-xr-x   0 micafer   (1000) micafer   (1000)        0 2024-05-30 06:19:12.215840 RADL-1.3.3/radl/
+-rw-r--r--   0 micafer   (1000) micafer   (1000)      804 2024-05-30 06:05:31.000000 RADL-1.3.3/radl/__init__.py
+-rw-r--r--   0 micafer   (1000) micafer   (1000)    54050 2024-05-30 06:05:31.000000 RADL-1.3.3/radl/radl.py
+-rw-r--r--   0 micafer   (1000) micafer   (1000)     8633 2024-05-30 06:05:31.000000 RADL-1.3.3/radl/radl_json.py
+-rw-r--r--   0 micafer   (1000) micafer   (1000)    12276 2024-05-30 06:05:31.000000 RADL-1.3.3/radl/radl_parse.py
+-rw-r--r--   0 micafer   (1000) micafer   (1000)       38 2024-05-30 06:19:12.215840 RADL-1.3.3/setup.cfg
+-rw-r--r--   0 micafer   (1000) micafer   (1000)     1627 2024-05-30 06:05:31.000000 RADL-1.3.3/setup.py
```

### Comparing `RADL-1.3.2/INSTALL` & `RADL-1.3.3/INSTALL`

 * *Files identical despite different names*

### Comparing `RADL-1.3.2/LICENSE` & `RADL-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RADL-1.3.2/NOTICE` & `RADL-1.3.3/NOTICE`

 * *Files identical despite different names*

### Comparing `RADL-1.3.2/PKG-INFO` & `RADL-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RADL
-Version: 1.3.2
+Version: 1.3.3
 Summary: Resource and Application Description Language (RADL) parser.
 Home-page: https://github.com/grycap/RADL
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: micafer1@upv.es
 License: GPL version 3, http://www.gnu.org/licenses/gpl-3.0.txt
 Platform: any
 License-File: LICENSE
```

### Comparing `RADL-1.3.2/RADL.egg-info/PKG-INFO` & `RADL-1.3.3/RADL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RADL
-Version: 1.3.2
+Version: 1.3.3
 Summary: Resource and Application Description Language (RADL) parser.
 Home-page: https://github.com/grycap/RADL
 Author: GRyCAP - Universitat Politecnica de Valencia
 Author-email: micafer1@upv.es
 License: GPL version 3, http://www.gnu.org/licenses/gpl-3.0.txt
 Platform: any
 License-File: LICENSE
```

### Comparing `RADL-1.3.2/README` & `RADL-1.3.3/README`

 * *Files identical despite different names*

### Comparing `RADL-1.3.2/changelog` & `RADL-1.3.3/changelog`

 * *Files 8% similar despite different names*

```diff
@@ -65,7 +65,13 @@
 RADL 1.31
 
     * Fix error: description is not returned in str of RADL.
 
 RADL 1.32
 
     * Error parsing net_interface.0.additional_dns_names in json.
+
+RADL 1.33
+
+    * Minor internal code changes.
+    * Add remove_net_interface function.
+
```

### Comparing `RADL-1.3.2/radl/__init__.py` & `RADL-1.3.3/radl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 __all__ = ['radl_parse', 'radl_json', 'radl']
-__version__ = '1.3.2'
+__version__ = '1.3.3'
```

### Comparing `RADL-1.3.2/radl/radl.py` & `RADL-1.3.3/radl/radl.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import copy
 import re
-from distutils.version import LooseVersion
+from packaging.version import Version
 
 try:
     unicode
 except Exception:
     unicode = bytes
 
 
@@ -793,15 +793,15 @@
     def isNewerThan(self, other):
         """ Compare if the version of this app is newer that the other """
         if self.getValue("name") == other.getValue("name"):
             if other.getValue("version"):
                 if not other.getValue("version"):
                     return False
                 else:
-                    return LooseVersion(self.getValue("version")) > LooseVersion(other.getValue("version"))
+                    return Version(self.getValue("version")) > Version(other.getValue("version"))
             else:
                 return True
         else:
             return False
 
     def check(self, radl):
         """Check the features in this application."""
@@ -926,14 +926,28 @@
         while True:
             netid = self.getValue("net_interface.%d.connection" % i)
             if not netid:
                 return res
             res.append(netid)
             i += 1
 
+    def remove_net_interface(self, iface_num):
+        """Remove the network interface with that number."""
+        for f in self.features:
+            if (f.prop.startswith("net_interface.%d" % iface_num)):
+                self.delValue(f.prop)
+
+        i = iface_num + 1
+        while self.getValue("net_interface.%d.connection" % i):
+            for f in self.features:
+                if (f.prop.startswith("net_interface.%d" % i)):
+                    self.setValue(f.prop.replace(str(i), str(i - 1)), f.value)
+                    self.delValue(f.prop)
+            i += 1
+
     def getCredentialValues(self, new=False):
         """Return the values in disk.0.os.credentials.*."""
 
         credentials_base = "disk.0.os.credentials."
         if new:
             credentials_base = "disk.0.os.credentials.new."
         return tuple([self.getValue(credentials_base + p) for p in [
@@ -1476,16 +1490,16 @@
         1:10/tcp,9:22/udp
         1:10,9:22
         Returns a list of outport objects
         """
         res = []
         ports = outports.split(',')
         for port in ports:
-            expr = ("^((\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3}\/\d{1,2})-){0,1}((\d+)((:)\d+){0,1}((\/tcp|\/udp){0,1}))"
-                    "((-)((\d+)((:)\d+){0,1}((\/tcp|\/udp){0,1}))){0,1}$")
+            expr = (r"^((\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3}\/\d{1,2})-){0,1}((\d+)((:)\d+){0,1}((\/tcp|\/udp){0,1}))"
+                    r"((-)((\d+)((:)\d+){0,1}((\/tcp|\/udp){0,1}))){0,1}$")
             match = re.search(expr, port)
             if not match:
                 raise RADLParseException('Invalid outports format.')
             groups = match.groups()
 
             local_protocol = groups[6][1:] if groups[6] else "tcp"
             remote_protocol = groups[14][1:] if groups[14] else local_protocol
```

### Comparing `RADL-1.3.2/radl/radl_json.py` & `RADL-1.3.3/radl/radl_json.py`

 * *Files identical despite different names*

### Comparing `RADL-1.3.2/radl/radl_parse.py` & `RADL-1.3.3/radl/radl_parse.py`

 * *Files identical despite different names*

### Comparing `RADL-1.3.2/setup.py` & `RADL-1.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,8 @@
       license="GPL version 3, http://www.gnu.org/licenses/gpl-3.0.txt",
       long_description=("The main purpose of the Resource and Application description Language (RADL) is "
                         "to specify the requirements of the scientific applications needed to be deployed "
                         "in a virtualized computational infrastructure (cloud). It is compatible with both "
                         "Python 2 and Python 3"),
       description="Resource and Application Description Language (RADL) parser.",
       platforms=["any"],
-      install_requires=["ply"])
+      install_requires=["ply", "packaging"])
```

