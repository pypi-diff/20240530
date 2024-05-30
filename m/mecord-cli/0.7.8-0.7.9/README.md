# Comparing `tmp/mecord-cli-0.7.8.tar.gz` & `tmp/mecord-cli-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecord-cli-0.7.8.tar", last modified: Wed Feb 28 08:31:07 2024, max compression
+gzip compressed data, was "mecord-cli-0.7.9.tar", last modified: Wed Feb 28 08:36:17 2024, max compression
```

## Comparing `mecord-cli-0.7.8.tar` & `mecord-cli-0.7.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 08:31:07.789537 mecord-cli-0.7.8/
--rw-rw-rw-   0        0        0     1078 2023-02-16 06:18:02.000000 mecord-cli-0.7.8/LICENSE
--rw-rw-rw-   0        0        0     2363 2024-02-28 08:31:07.789537 mecord-cli-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0     1942 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 08:31:07.764971 mecord-cli-0.7.8/mecord/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/__init__.py
--rw-rw-rw-   0        0        0      171 2024-02-28 08:31:06.000000 mecord-cli-0.7.8/mecord/constant.py
--rw-rw-rw-   0        0        0    13041 2024-02-28 08:30:35.000000 mecord-cli-0.7.8/mecord/main.py
--rw-rw-rw-   0        0        0    14338 2024-02-28 07:47:37.000000 mecord-cli-0.7.8/mecord/mecord_server_socket.py
--rw-rw-rw-   0        0        0    10821 2024-02-28 08:00:49.000000 mecord-cli-0.7.8/mecord/mecord_service.py
--rw-rw-rw-   0        0        0    16362 2024-02-28 03:53:51.000000 mecord-cli-0.7.8/mecord/mecord_widget.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:31:07.777522 mecord-cli-0.7.8/mecord/pb/
--rw-rw-rw-   0        0        0        0 2023-11-30 13:43:12.000000 mecord-cli-0.7.8/mecord/pb/__init__.py
--rw-rw-rw-   0        0        0   100471 2024-01-26 10:15:58.000000 mecord-cli-0.7.8/mecord/pb/aigc_ext_pb2.py
--rw-rw-rw-   0        0        0    42678 2024-01-26 10:15:56.000000 mecord-cli-0.7.8/mecord/pb/aigc_int_pb2.py
--rw-rw-rw-   0        0        0     5167 2024-01-26 10:15:53.000000 mecord-cli-0.7.8/mecord/pb/cmd_id_ext_pb2.py
--rw-rw-rw-   0        0        0    45667 2024-01-26 10:15:15.000000 mecord-cli-0.7.8/mecord/pb/common_ext_pb2.py
--rw-rw-rw-   0        0        0    26039 2024-01-26 10:15:15.000000 mecord-cli-0.7.8/mecord/pb/interaction_int_pb2.py
--rw-rw-rw-   0        0        0   126580 2024-01-26 10:15:49.000000 mecord-cli-0.7.8/mecord/pb/mecord_ext_pb2.py
--rw-rw-rw-   0        0        0    23579 2024-01-26 10:15:44.000000 mecord-cli-0.7.8/mecord/pb/message_ext_pb2.py
--rw-rw-rw-   0        0        0     3250 2024-01-26 10:15:15.000000 mecord-cli-0.7.8/mecord/pb/rpcinput_pb2.py
--rw-rw-rw-   0        0        0     9808 2024-01-26 10:15:41.000000 mecord-cli-0.7.8/mecord/pb/search_ext_pb2.py
--rw-rw-rw-   0        0        0    56233 2024-01-26 10:15:39.000000 mecord-cli-0.7.8/mecord/pb/studio_ext_pb2.py
--rw-rw-rw-   0        0        0     3387 2024-01-26 10:15:15.000000 mecord-cli-0.7.8/mecord/pb/tarsproxy_pb2.py
--rw-rw-rw-   0        0        0     9438 2024-01-26 10:15:15.000000 mecord-cli-0.7.8/mecord/pb/uauth_common_pb2.py
--rw-rw-rw-   0        0        0   116141 2024-01-26 10:15:34.000000 mecord-cli-0.7.8/mecord/pb/uauth_ext_pb2.py
--rw-rw-rw-   0        0        0    44399 2024-01-26 10:16:02.000000 mecord-cli-0.7.8/mecord/pb/user_ext_pb2.py
--rw-rw-rw-   0        0        0    12847 2024-01-26 10:16:00.000000 mecord-cli-0.7.8/mecord/pb/user_status_ext_pb2.py
--rw-rw-rw-   0        0        0    10668 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/progress_monitor.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:31:07.781031 mecord-cli-0.7.8/mecord/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/script_template/__init__.py
--rw-rw-rw-   0        0        0      312 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/script_template/launch.py
--rw-rw-rw-   0        0        0      915 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/script_template/main.py
--rw-rw-rw-   0        0        0      801 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/script_template/run.py
--rw-rw-rw-   0        0        0     9424 2024-02-04 03:14:26.000000 mecord-cli-0.7.8/mecord/server_func.py
--rw-rw-rw-   0        0        0     5357 2024-02-28 03:31:29.000000 mecord-cli-0.7.8/mecord/store.py
--rw-rw-rw-   0        0        0     9256 2024-02-28 03:45:40.000000 mecord-cli-0.7.8/mecord/task.py
--rw-rw-rw-   0        0        0    11105 2024-02-28 03:19:16.000000 mecord-cli-0.7.8/mecord/taskUtils.py
--rw-rw-rw-   0        0        0     6012 2024-02-04 03:14:25.000000 mecord-cli-0.7.8/mecord/upload.py
--rw-rw-rw-   0        0        0    10880 2024-02-28 03:57:30.000000 mecord-cli-0.7.8/mecord/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:31:07.784031 mecord-cli-0.7.8/mecord/widget_template/
--rw-rw-rw-   0        0        0     1977 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/widget_template/MekongJS.js.py
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/widget_template/__init__.py
--rw-rw-rw-   0        0        0      219 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/widget_template/config.json.py
--rw-rw-rw-   0        0        0     1678 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/widget_template/icon.png.py
--rw-rw-rw-   0        0        0      719 2023-10-11 09:27:31.000000 mecord-cli-0.7.8/mecord/widget_template/index.html.py
--rw-rw-rw-   0        0        0     5293 2024-02-28 07:42:20.000000 mecord-cli-0.7.8/mecord/xy_network.py
--rw-rw-rw-   0        0        0    13553 2024-02-28 07:54:24.000000 mecord-cli-0.7.8/mecord/xy_pb.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:31:07.788533 mecord-cli-0.7.8/mecord_cli.egg-info/
--rw-rw-rw-   0        0        0     2363 2024-02-28 08:31:07.000000 mecord-cli-0.7.8/mecord_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1292 2024-02-28 08:31:07.000000 mecord-cli-0.7.8/mecord_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 08:31:07.000000 mecord-cli-0.7.8/mecord_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-02-28 08:31:07.000000 mecord-cli-0.7.8/mecord_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      170 2024-02-28 08:31:07.000000 mecord-cli-0.7.8/mecord_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-02-28 08:31:07.000000 mecord-cli-0.7.8/mecord_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-28 08:31:07.790541 mecord-cli-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     2709 2024-02-28 08:30:59.000000 mecord-cli-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-28 08:36:17.109825 mecord-cli-0.7.9/
+-rw-rw-rw-   0        0        0     1078 2023-02-16 06:18:02.000000 mecord-cli-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0     2363 2024-02-28 08:36:17.109825 mecord-cli-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1942 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-28 08:36:17.083267 mecord-cli-0.7.9/mecord/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/__init__.py
+-rw-rw-rw-   0        0        0      171 2024-02-28 08:36:16.000000 mecord-cli-0.7.9/mecord/constant.py
+-rw-rw-rw-   0        0        0    13045 2024-02-28 08:36:04.000000 mecord-cli-0.7.9/mecord/main.py
+-rw-rw-rw-   0        0        0    14338 2024-02-28 07:47:37.000000 mecord-cli-0.7.9/mecord/mecord_server_socket.py
+-rw-rw-rw-   0        0        0    10821 2024-02-28 08:00:49.000000 mecord-cli-0.7.9/mecord/mecord_service.py
+-rw-rw-rw-   0        0        0    16362 2024-02-28 03:53:51.000000 mecord-cli-0.7.9/mecord/mecord_widget.py
+drwxrwxrwx   0        0        0        0 2024-02-28 08:36:17.094789 mecord-cli-0.7.9/mecord/pb/
+-rw-rw-rw-   0        0        0        0 2023-11-30 13:43:12.000000 mecord-cli-0.7.9/mecord/pb/__init__.py
+-rw-rw-rw-   0        0        0   100471 2024-01-26 10:15:58.000000 mecord-cli-0.7.9/mecord/pb/aigc_ext_pb2.py
+-rw-rw-rw-   0        0        0    42678 2024-01-26 10:15:56.000000 mecord-cli-0.7.9/mecord/pb/aigc_int_pb2.py
+-rw-rw-rw-   0        0        0     5167 2024-01-26 10:15:53.000000 mecord-cli-0.7.9/mecord/pb/cmd_id_ext_pb2.py
+-rw-rw-rw-   0        0        0    45667 2024-01-26 10:15:15.000000 mecord-cli-0.7.9/mecord/pb/common_ext_pb2.py
+-rw-rw-rw-   0        0        0    26039 2024-01-26 10:15:15.000000 mecord-cli-0.7.9/mecord/pb/interaction_int_pb2.py
+-rw-rw-rw-   0        0        0   126580 2024-01-26 10:15:49.000000 mecord-cli-0.7.9/mecord/pb/mecord_ext_pb2.py
+-rw-rw-rw-   0        0        0    23579 2024-01-26 10:15:44.000000 mecord-cli-0.7.9/mecord/pb/message_ext_pb2.py
+-rw-rw-rw-   0        0        0     3250 2024-01-26 10:15:15.000000 mecord-cli-0.7.9/mecord/pb/rpcinput_pb2.py
+-rw-rw-rw-   0        0        0     9808 2024-01-26 10:15:41.000000 mecord-cli-0.7.9/mecord/pb/search_ext_pb2.py
+-rw-rw-rw-   0        0        0    56233 2024-01-26 10:15:39.000000 mecord-cli-0.7.9/mecord/pb/studio_ext_pb2.py
+-rw-rw-rw-   0        0        0     3387 2024-01-26 10:15:15.000000 mecord-cli-0.7.9/mecord/pb/tarsproxy_pb2.py
+-rw-rw-rw-   0        0        0     9438 2024-01-26 10:15:15.000000 mecord-cli-0.7.9/mecord/pb/uauth_common_pb2.py
+-rw-rw-rw-   0        0        0   116141 2024-01-26 10:15:34.000000 mecord-cli-0.7.9/mecord/pb/uauth_ext_pb2.py
+-rw-rw-rw-   0        0        0    44399 2024-01-26 10:16:02.000000 mecord-cli-0.7.9/mecord/pb/user_ext_pb2.py
+-rw-rw-rw-   0        0        0    12847 2024-01-26 10:16:00.000000 mecord-cli-0.7.9/mecord/pb/user_status_ext_pb2.py
+-rw-rw-rw-   0        0        0    10668 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/progress_monitor.py
+drwxrwxrwx   0        0        0        0 2024-02-28 08:36:17.098304 mecord-cli-0.7.9/mecord/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/script_template/__init__.py
+-rw-rw-rw-   0        0        0      312 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/script_template/launch.py
+-rw-rw-rw-   0        0        0      915 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/script_template/main.py
+-rw-rw-rw-   0        0        0      801 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/script_template/run.py
+-rw-rw-rw-   0        0        0     9424 2024-02-04 03:14:26.000000 mecord-cli-0.7.9/mecord/server_func.py
+-rw-rw-rw-   0        0        0     5357 2024-02-28 03:31:29.000000 mecord-cli-0.7.9/mecord/store.py
+-rw-rw-rw-   0        0        0     9256 2024-02-28 03:45:40.000000 mecord-cli-0.7.9/mecord/task.py
+-rw-rw-rw-   0        0        0    11105 2024-02-28 03:19:16.000000 mecord-cli-0.7.9/mecord/taskUtils.py
+-rw-rw-rw-   0        0        0     6012 2024-02-04 03:14:25.000000 mecord-cli-0.7.9/mecord/upload.py
+-rw-rw-rw-   0        0        0    10880 2024-02-28 03:57:30.000000 mecord-cli-0.7.9/mecord/utils.py
+drwxrwxrwx   0        0        0        0 2024-02-28 08:36:17.102314 mecord-cli-0.7.9/mecord/widget_template/
+-rw-rw-rw-   0        0        0     1977 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/widget_template/MekongJS.js.py
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/widget_template/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/widget_template/config.json.py
+-rw-rw-rw-   0        0        0     1678 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/widget_template/icon.png.py
+-rw-rw-rw-   0        0        0      719 2023-10-11 09:27:31.000000 mecord-cli-0.7.9/mecord/widget_template/index.html.py
+-rw-rw-rw-   0        0        0     5293 2024-02-28 07:42:20.000000 mecord-cli-0.7.9/mecord/xy_network.py
+-rw-rw-rw-   0        0        0    13553 2024-02-28 07:54:24.000000 mecord-cli-0.7.9/mecord/xy_pb.py
+drwxrwxrwx   0        0        0        0 2024-02-28 08:36:17.108817 mecord-cli-0.7.9/mecord_cli.egg-info/
+-rw-rw-rw-   0        0        0     2363 2024-02-28 08:36:16.000000 mecord-cli-0.7.9/mecord_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1292 2024-02-28 08:36:17.000000 mecord-cli-0.7.9/mecord_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-28 08:36:16.000000 mecord-cli-0.7.9/mecord_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-02-28 08:36:16.000000 mecord-cli-0.7.9/mecord_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      170 2024-02-28 08:36:16.000000 mecord-cli-0.7.9/mecord_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-02-28 08:36:16.000000 mecord-cli-0.7.9/mecord_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-28 08:36:17.110832 mecord-cli-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     2709 2024-02-28 08:35:30.000000 mecord-cli-0.7.9/setup.py
```

### Comparing `mecord-cli-0.7.8/LICENSE` & `mecord-cli-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/PKG-INFO` & `mecord-cli-0.7.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.7.8
+Version: 0.7.9
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mecord-cli-0.7.8/README.md` & `mecord-cli-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/main.py` & `mecord-cli-0.7.9/mecord/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from mecord import mecord_service
 from mecord import mecord_widget
 from mecord import store
 from mecord import utils
 from mecord import taskUtils
 from mecord import xy_pb
 
-ll = 40
+ll = 42
 def scr_str(s):
     return "| " + s + " |"
 def scr_str1(s):
     return "| " + s
 def scr_line(s):
     return "|" + s + "|"
 
@@ -52,16 +52,16 @@
                 real_s = this_lst[this_d]
                 if len(append_str) > 0:
                     real_s += f" [{append_str}]"
                 real_stdsrc(row_idx, col_idx, scr_str(" " + real_s.ljust(ll-1)))
             else:
                 real_stdsrc(row_idx, col_idx, scr_str(" " + " ".ljust(ll-1)))
         widget_stdscr(d, test_lst, idx, 0, "test" if platform.system() == 'Windows' else "")
-        widget_stdscr(d, us_lst, idx, ll*1, "us" if platform.system() == 'Windows' else "")
-        widget_stdscr(d, sg_lst, idx, ll*2, "sg" if platform.system() == 'Windows' else "")
+        widget_stdscr(d, us_lst, idx, ll*1-1, "us" if platform.system() == 'Windows' else "")
+        widget_stdscr(d, sg_lst, idx, ll*2-2, "sg" if platform.system() == 'Windows' else "")
         idx+=1
     return idx
 
 def device_status(stdscr, idx):
     def real_stdsrc(*args):
         if platform.system() == 'Windows':
             print(args[2])
```

### Comparing `mecord-cli-0.7.8/mecord/mecord_server_socket.py` & `mecord-cli-0.7.9/mecord/mecord_server_socket.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/mecord_service.py` & `mecord-cli-0.7.9/mecord/mecord_service.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/mecord_widget.py` & `mecord-cli-0.7.9/mecord/mecord_widget.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/aigc_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/aigc_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/aigc_int_pb2.py` & `mecord-cli-0.7.9/mecord/pb/aigc_int_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/cmd_id_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/cmd_id_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/common_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/common_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/interaction_int_pb2.py` & `mecord-cli-0.7.9/mecord/pb/interaction_int_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/mecord_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/mecord_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/message_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/message_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/rpcinput_pb2.py` & `mecord-cli-0.7.9/mecord/pb/rpcinput_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/search_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/search_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/studio_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/studio_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/tarsproxy_pb2.py` & `mecord-cli-0.7.9/mecord/pb/tarsproxy_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/uauth_common_pb2.py` & `mecord-cli-0.7.9/mecord/pb/uauth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/uauth_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/uauth_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/user_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/user_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/pb/user_status_ext_pb2.py` & `mecord-cli-0.7.9/mecord/pb/user_status_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/progress_monitor.py` & `mecord-cli-0.7.9/mecord/progress_monitor.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/script_template/main.py` & `mecord-cli-0.7.9/mecord/script_template/main.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/script_template/run.py` & `mecord-cli-0.7.9/mecord/script_template/run.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/server_func.py` & `mecord-cli-0.7.9/mecord/server_func.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/store.py` & `mecord-cli-0.7.9/mecord/store.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/task.py` & `mecord-cli-0.7.9/mecord/task.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/taskUtils.py` & `mecord-cli-0.7.9/mecord/taskUtils.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/upload.py` & `mecord-cli-0.7.9/mecord/upload.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/utils.py` & `mecord-cli-0.7.9/mecord/utils.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/widget_template/MekongJS.js.py` & `mecord-cli-0.7.9/mecord/widget_template/MekongJS.js.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/widget_template/icon.png.py` & `mecord-cli-0.7.9/mecord/widget_template/icon.png.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/widget_template/index.html.py` & `mecord-cli-0.7.9/mecord/widget_template/index.html.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/xy_network.py` & `mecord-cli-0.7.9/mecord/xy_network.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord/xy_pb.py` & `mecord-cli-0.7.9/mecord/xy_pb.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/mecord_cli.egg-info/PKG-INFO` & `mecord-cli-0.7.9/mecord_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.7.8
+Version: 0.7.9
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mecord-cli-0.7.8/mecord_cli.egg-info/SOURCES.txt` & `mecord-cli-0.7.9/mecord_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.7.8/setup.py` & `mecord-cli-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-mecord_version = "0.7.8"
+mecord_version = "0.7.9"
 mecord_build_number = int(mecord_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "mecord", "constant.py")
 try:
     result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     if result.returncode == 0:
```

