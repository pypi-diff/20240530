# Comparing `tmp/python_115-0.0.8.7.tar.gz` & `tmp/python_115-0.0.8.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.7.tar", max compression
+gzip compressed data, was "python_115-0.0.8.7.1.tar", max compression
```

## Comparing `python_115-0.0.8.7.tar` & `python_115-0.0.8.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.7/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.7/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2130 2024-05-29 04:11:20.077720 python_115-0.0.8.7/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7/p115/component/cipher.py
--rwxr-xr-x   0        0        0   259974 2024-05-30 05:46:47.226617 python_115-0.0.8.7/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7/p115/component/exception.py
--rwxr-xr-x   0        0        0    66130 2024-05-28 15:26:11.565966 python_115-0.0.8.7/p115/component/fs.py
--rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.7/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.7/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.7/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.7/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7/p115/py.typed
--rwxr-xr-x   0        0        0     8620 2024-05-30 06:00:02.651353 python_115-0.0.8.7/p115/tool/__init__.py
--rw-r--r--   0        0        0     1679 2024-05-30 06:00:27.500175 python_115-0.0.8.7/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.7/readme.md
--rw-r--r--   0        0        0    36397 1970-01-01 00:00:00.000000 python_115-0.0.8.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7.1/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7.1/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7.1/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7.1/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.7.1/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7.1/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.7.1/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2130 2024-05-29 04:11:20.077720 python_115-0.0.8.7.1/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7.1/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7.1/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7.1/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7.1/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   259970 2024-05-30 06:11:29.409434 python_115-0.0.8.7.1/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7.1/p115/component/exception.py
+-rwxr-xr-x   0        0        0    66130 2024-05-28 15:26:11.565966 python_115-0.0.8.7.1/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.7.1/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.7.1/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.7.1/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7.1/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.7.1/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7.1/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7.1/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7.1/p115/py.typed
+-rwxr-xr-x   0        0        0     8620 2024-05-30 06:05:30.073930 python_115-0.0.8.7.1/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1681 2024-05-30 06:11:36.221279 python_115-0.0.8.7.1/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.7.1/readme.md
+-rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.7.1/PKG-INFO
```

### Comparing `python_115-0.0.8.7/LICENSE` & `python_115-0.0.8.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/cmd/check.py` & `python_115-0.0.8.7.1/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/cmd/iterdir.py` & `python_115-0.0.8.7.1/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/cmd/qrcode.py` & `python_115-0.0.8.7.1/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/__init__.py` & `python_115-0.0.8.7.1/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/cipher.py` & `python_115-0.0.8.7.1/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/client.py` & `python_115-0.0.8.7.1/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -7108,15 +7108,15 @@
         payload:
             - ids: int | str # 助愿的 id，多个用逗号 "," 隔开
         """
         api = "https://act.115.com/api/1.0/web/1.0/act2024xys/del_aid_desire"
         if isinstance(payload, (int, str)):
             payload = {"ids": payload}
         request_kwargs.pop("parse", None)
-        return self.request(api, "POST", params=payload, async_=async_, **request_kwargs)
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     @overload
     def act_xys_get_desire_info(
         self, 
         payload: str | dict, 
         /,
         async_: Literal[False] = False, 
@@ -7222,15 +7222,15 @@
         payload:
             - did: str # 许愿的 id
             - aid: int | str # 助愿的 id
             - to_cid: int = <default> # 助愿中的分享链接转存到你的网盘中目录的 id
         """
         api = "https://act.115.com/api/1.0/web/1.0/act2024xys/adopt"
         request_kwargs.pop("parse", None)
-        return self.request(api, "POST", params=payload, async_=async_, **request_kwargs)
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     ########## Other Encapsulations ##########
 
     # TODO 支持异步
     @overload
     def open(
         self,
```

### Comparing `python_115-0.0.8.7/p115/component/fs.py` & `python_115-0.0.8.7.1/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/fs_base.py` & `python_115-0.0.8.7.1/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/fs_share.py` & `python_115-0.0.8.7.1/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/fs_zip.py` & `python_115-0.0.8.7.1/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/labellist.py` & `python_115-0.0.8.7.1/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/offline.py` & `python_115-0.0.8.7.1/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/recyclebin.py` & `python_115-0.0.8.7.1/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/component/sharing.py` & `python_115-0.0.8.7.1/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/p115/tool/__init__.py` & `python_115-0.0.8.7.1/p115/tool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 ) -> str:
     """许愿树活动：创建助愿（助愿创建后需要等审核）
     :param client: 115 客户端
     :param wish_id: 许愿 id
     :param content: 助愿内容
     :param file_ids: 文件在你的网盘的 id，多个用逗号 "," 隔开
 
-    :return: 祝愿 id
+    :return: 助愿 id
     """
     if isinstance(client, str):
         client = P115Client(client)
     if not isinstance(file_ids, (int, str)):
         file_ids = ",".join(map(str, file_ids))
     return check_response(
         client.act_xys_aid_desire({"id": wish_id, "content": content, "file_ids": file_ids}
@@ -233,13 +233,13 @@
     aid_id: int | str, 
     to_cid: int = 0, 
 ) -> dict:
     """许愿树活动：采纳助愿
     :param client: 115 客户端
     :param wish_id: 许愿 id
     :param aid_id: 助愿 id
-    :param to_cid: 祝愿的分享文件保存到你的网盘中目录的 id
+    :param to_cid: 助愿的分享文件保存到你的网盘中目录的 id
     """
     if isinstance(client, str):
         client = P115Client(client)
     return check_response(client.act_xys_adopt({"did": wish_id, "aid": aid_id, "to_cid": to_cid}))
```

### Comparing `python_115-0.0.8.7/pyproject.toml` & `python_115-0.0.8.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.7"
+version = "0.0.8.7.1"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.7/readme.md` & `python_115-0.0.8.7.1/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.7/PKG-INFO` & `python_115-0.0.8.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.7
+Version: 0.0.8.7.1
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

