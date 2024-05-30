# Comparing `tmp/xingpyc-0.2.6.tar.gz` & `tmp/xingpyc-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.2.6.tar", last modified: Thu May 30 07:16:51 2024, max compression
+gzip compressed data, was "xingpyc-0.2.7.tar", last modified: Thu May 30 07:22:39 2024, max compression
```

## Comparing `xingpyc-0.2.6.tar` & `xingpyc-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.095384 xingpyc-0.2.6/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:16:51.095133 xingpyc-0.2.6/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.6/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-30 07:16:40.000000 xingpyc-0.2.6/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-30 07:16:51.095439 xingpyc-0.2.6/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.093523 xingpyc-0.2.6/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.094075 xingpyc-0.2.6/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)    10113 2024-05-30 07:16:44.000000 xingpyc-0.2.6/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.6/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.094933 xingpyc-0.2.6/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-30 07:16:51.000000 xingpyc-0.2.6/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:16:51.094767 xingpyc-0.2.6/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.6/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:22:39.734131 xingpyc-0.2.7/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:22:39.733910 xingpyc-0.2.7/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.7/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-30 07:22:37.000000 xingpyc-0.2.7/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-30 07:22:39.734200 xingpyc-0.2.7/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:22:39.732323 xingpyc-0.2.7/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:22:39.732876 xingpyc-0.2.7/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)    10187 2024-05-30 07:22:29.000000 xingpyc-0.2.7/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.7/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:22:39.733694 xingpyc-0.2.7/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-30 07:22:39.000000 xingpyc-0.2.7/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-30 07:22:39.000000 xingpyc-0.2.7/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-30 07:22:39.000000 xingpyc-0.2.7/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-30 07:22:39.000000 xingpyc-0.2.7/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-30 07:22:39.000000 xingpyc-0.2.7/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-30 07:22:39.733555 xingpyc-0.2.7/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.7/tests/test1.py
```

### Comparing `xingpyc-0.2.6/PKG-INFO` & `xingpyc-0.2.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.2.6/pyproject.toml` & `xingpyc-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.2.6/src/xingpyc/__init__.py` & `xingpyc-0.2.7/src/xingpyc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,19 @@
             if loopCount % 50 == 0 and self.cloudClient is not None:
                 self.cloudClient.send_bytes("check     0000000000")
                 print("check to cloud")
 
             ### here starts the incoming message processing
             ### here starts the incoming message processing
             ### here starts the incoming message processing
-            currentMsg = self.incomingMsg
-            self.incomingMsg = []
+
+            currentMsg = []
+            while len(self.incomingMsg) != 0:
+                currentMsg.append(self.incomingMsg.pop())
+                
             for client_id, message in currentMsg:
                 print(
                     "\033[93mheader:"+
                     message[:10].replace(b" ", b"").decode()+
                     "   id:"+
                     message[10:20].decode()+
                     "   length:"+
```

### Comparing `xingpyc-0.2.6/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.2.7/src/xingpyc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.6
+Version: 0.2.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

