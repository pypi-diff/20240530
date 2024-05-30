# Comparing `tmp/pyiotown-0.5.2-py3-none-any.whl.zip` & `tmp/pyiotown-0.5.3.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 8371 bytes, number of entries: 12
+Zip file size: 8664 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-05 08:55 pyiotown/__init__.py
 -rw-r--r--  2.0 unx      795 b- defN 24-Apr-30 13:17 pyiotown/command.py
 -rw-r--r--  2.0 unx      925 b- defN 23-Sep-04 05:59 pyiotown/delete.py
 -rw-r--r--  2.0 unx     4313 b- defN 24-Mar-21 23:18 pyiotown/get.py
 -rw-r--r--  2.0 unx     5058 b- defN 23-Sep-04 06:00 pyiotown/post.py
--rw-r--r--  2.0 unx     8447 b- defN 24-Apr-22 22:44 pyiotown/post_process.py
--rw-r--r--  2.0 unx     1053 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      696 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/pbr.json
--rw-r--r--  2.0 unx        9 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      926 b- defN 24-May-01 22:28 pyiotown-0.5.2.dist-info/RECORD
-12 files, 22361 bytes uncompressed, 6819 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx     8151 b- defN 24-May-30 12:23 pyiotown/post_process.py
+-rw-r--r--  2.0 unx     1053 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      699 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       47 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/pbr.json
+-rw-r--r--  2.0 unx        9 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1057 b- defN 24-May-30 12:35 pyiotown-0.5.3.dev1.dist-info/RECORD
+13 files, 22248 bytes uncompressed, 6884 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -12,26 +12,29 @@
 
 Filename: pyiotown/post.py
 Comment: 
 
 Filename: pyiotown/post_process.py
 Comment: 
 
-Filename: pyiotown-0.5.2.dist-info/LICENSE
+Filename: pyiotown-0.5.3.dev1.dist-info/LICENSE
 Comment: 
 
-Filename: pyiotown-0.5.2.dist-info/METADATA
+Filename: pyiotown-0.5.3.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pyiotown-0.5.2.dist-info/WHEEL
+Filename: pyiotown-0.5.3.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pyiotown-0.5.2.dist-info/pbr.json
+Filename: pyiotown-0.5.3.dev1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyiotown-0.5.2.dist-info/top_level.txt
+Filename: pyiotown-0.5.3.dev1.dist-info/pbr.json
 Comment: 
 
-Filename: pyiotown-0.5.2.dist-info/RECORD
+Filename: pyiotown-0.5.3.dev1.dist-info/top_level.txt
+Comment: 
+
+Filename: pyiotown-0.5.3.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyiotown/post_process.py

```diff
@@ -98,30 +98,21 @@
     timer = threading.Timer(60, updateExpire, [url, token, name, verify, timeout])
     timer.start()
 
 def getTopic(url, token, name, verify=True, timeout=60):
     apiaddr = url + "/api/v1.0/pp/proc"
     header = {'Accept':'application/json', 'token':token}
     payload = {'name':name}    
-    try:
-        r = requests.post(apiaddr, json=payload, headers=header, verify=verify, timeout=timeout)
-        if r.status_code == 200:
-            topic = json.loads((r.content).decode('utf-8'))['topic']
-            #print(f"Get Topic From IoT.own Success: {topic}")
-            return topic
-        elif r.status_code == 403:
-            topic = json.loads((r.content).decode('utf-8'))['topic']
-            #print(f"process already in use. please restart after 1 minute later.: {topic}")
-            return topic
-        else:
-            print(r)
-            return None
-    except Exception as e:
-        print(e)
-        return None
+
+    r = requests.post(apiaddr, json=payload, headers=header, verify=verify, timeout=timeout)
+    if r.status_code == 200 or r.status_code == 403: # Same with 200 (deprecated)
+        topic = json.loads((r.content).decode('utf-8'))['topic']
+        return topic
+    else:
+        raise Exception(r.content.decode('utf-8'))
 
 def connect(url, name, func, mqtt_url=None, verify=True, dry_run=False):
     url_parsed = urlparse(url)
     if url_parsed.username is None:
         raise Exception("The username is not specified.")
     username = url_parsed.username
 
@@ -133,15 +124,15 @@
     if url_parsed.port is not None:
         url += f":{url_parsed.port}"
     
     # get Topic From IoTown
     topic = getTopic(url, token, name, verify)
 
     if topic == None:
-        raise Exception("IoT.own returned none")
+        raise Exception("The server does not assign a topic for you.")
 
     try:
         group = topic.split('/')[2]
     except Exception as e:
         raise Exception(f"Invalid topic {topic}")
     
     updateExpire(url, token, name, verify)
```

## Comparing `pyiotown-0.5.2.dist-info/LICENSE` & `pyiotown-0.5.3.dev1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyiotown-0.5.2.dist-info/METADATA` & `pyiotown-0.5.3.dev1.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyiotown
-Version: 0.5.2
-Summary: IoT.own Library
+Version: 0.5.3.dev1
+Summary: IOTOWN Library
 Home-page: https://github.com/CoXlabInc/pyiotow
 Author: CoXlab Inc.
 Author-email: support@coxlab.kr
 Maintainer: Jongsoo Jeong
 Maintainer-email: jsjeong@coxlab.k
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoXlabInc/pyiotown/issues
@@ -17,8 +17,8 @@
 License-File: LICENSE
 Requires-Dist: pbr
 Requires-Dist: setuptools
 Requires-Dist: wheel
 Requires-Dist: requests
 Requires-Dist: paho-mqtt >=2.0.0
 
-IoT.own Library
+IOTOWN Library
```

## Comparing `pyiotown-0.5.2.dist-info/RECORD` & `pyiotown-0.5.3.dev1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 pyiotown/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyiotown/command.py,sha256=JpR_POwNd6QedRxeF8OinFN2JU16I6JmXmjU493brgQ,795
 pyiotown/delete.py,sha256=9lGaAQd6WOVPXnZxmq424edB_GFxUR_Ejs3uuAmsRIY,925
 pyiotown/get.py,sha256=Oa95zsi-bBiWeiy_3BQ5WPEl9TBS1CWSlFBVoNUgZkY,4313
 pyiotown/post.py,sha256=hU9umOVXp59NdDxuTZYApBG2hPGBuKs2hpoHbbRrTt4,5058
-pyiotown/post_process.py,sha256=ISaVJfsesCyQoiTJvuV7M6GetnWmMlncImfzW65h5lo,8447
-pyiotown-0.5.2.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
-pyiotown-0.5.2.dist-info/METADATA,sha256=BiYWej7z7yLnWfhquVAXvIJzjnYySzGT-s77kpPd1I8,696
-pyiotown-0.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyiotown-0.5.2.dist-info/pbr.json,sha256=kv4cjETm7Ob9i2qncxrA7QhZ0xmkjeOluO6HkKKVPk4,47
-pyiotown-0.5.2.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
-pyiotown-0.5.2.dist-info/RECORD,,
+pyiotown/post_process.py,sha256=GWR8BVLW-dRMeA59CJSlLvqGtBFScAslxf2iYCxI_TY,8151
+pyiotown-0.5.3.dev1.dist-info/LICENSE,sha256=hf-g3asB2eVCMfAdxFSFlGUmBqk8KhH3U04FUvwOFGU,1053
+pyiotown-0.5.3.dev1.dist-info/METADATA,sha256=oP40IWW4vSdTnWuYFPDV2aVtVLeqU1CIsYc-8HO4xyY,699
+pyiotown-0.5.3.dev1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyiotown-0.5.3.dev1.dist-info/entry_points.txt,sha256=d3BnTxvZRnNv39gKdsIev-HjErkvzlq5ijynUxMVVEc,49
+pyiotown-0.5.3.dev1.dist-info/pbr.json,sha256=359X1KYW0tU_WieG2H5uPWb62MqGMA8HxUsfTM9CjGw,47
+pyiotown-0.5.3.dev1.dist-info/top_level.txt,sha256=7C_yB2E4KedHWqWClKpbaMmv2nYswwQ19MHhsBDr6kk,9
+pyiotown-0.5.3.dev1.dist-info/RECORD,,
```

