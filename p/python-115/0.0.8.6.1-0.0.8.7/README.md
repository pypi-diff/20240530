# Comparing `tmp/python_115-0.0.8.6.1.tar.gz` & `tmp/python_115-0.0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.6.1.tar", max compression
+gzip compressed data, was "python_115-0.0.8.7.tar", max compression
```

## Comparing `python_115-0.0.8.6.1.tar` & `python_115-0.0.8.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.6.1/LICENSE
--rwxr-xr-x   0        0        0      475 2024-05-29 04:25:59.676244 python_115-0.0.8.6.1/p115/__init__.py
--rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.6.1/p115/__main__.py
--rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.6.1/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.6.1/p115/cmd/check.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.6.1/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.6.1/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     2130 2024-05-29 04:11:20.077720 python_115-0.0.8.6.1/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.6.1/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.6.1/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.6.1/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.6.1/p115/component/cipher.py
--rwxr-xr-x   0        0        0   247309 2024-05-29 04:08:31.539577 python_115-0.0.8.6.1/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.6.1/p115/component/exception.py
--rwxr-xr-x   0        0        0    66130 2024-05-28 15:26:11.565966 python_115-0.0.8.6.1/p115/component/fs.py
--rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.6.1/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.6.1/p115/component/fs_share.py
--rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.6.1/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.6.1/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.6.1/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.6.1/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.6.1/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.6.1/p115/py.typed
--rwxr-xr-x   0        0        0     5494 2024-05-29 04:08:58.019283 python_115-0.0.8.6.1/p115/tool/__init__.py
--rw-r--r--   0        0        0     1681 2024-05-29 04:26:24.027670 python_115-0.0.8.6.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.6.1/readme.md
--rw-r--r--   0        0        0    36399 1970-01-01 00:00:00.000000 python_115-0.0.8.6.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.7/LICENSE
+-rwxr-xr-x   0        0        0      475 2024-05-30 06:00:49.607382 python_115-0.0.8.7/p115/__init__.py
+-rwxr-xr-x   0        0        0      243 2024-05-28 12:34:40.393193 python_115-0.0.8.7/p115/__main__.py
+-rwxr-xr-x   0        0        0      182 2024-05-28 08:48:54.248098 python_115-0.0.8.7/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0     1749 2024-05-28 08:50:02.907526 python_115-0.0.8.7/p115/cmd/check.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.7/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8856 2024-05-28 08:51:03.570423 python_115-0.0.8.7/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     2130 2024-05-29 04:11:20.077720 python_115-0.0.8.7/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.7/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.7/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1574 2024-05-28 12:32:04.087155 python_115-0.0.8.7/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.7/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   259974 2024-05-30 05:46:47.226617 python_115-0.0.8.7/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.7/p115/component/exception.py
+-rwxr-xr-x   0        0        0    66130 2024-05-28 15:26:11.565966 python_115-0.0.8.7/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48262 2024-05-28 15:24:40.699422 python_115-0.0.8.7/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    13897 2024-05-27 16:41:15.699681 python_115-0.0.8.7/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0    10058 2024-05-27 16:44:20.330025 python_115-0.0.8.7/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.7/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.7/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.7/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.7/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.7/p115/py.typed
+-rwxr-xr-x   0        0        0     8620 2024-05-30 06:00:02.651353 python_115-0.0.8.7/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1679 2024-05-30 06:00:27.500175 python_115-0.0.8.7/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.7/readme.md
+-rw-r--r--   0        0        0    36397 1970-01-01 00:00:00.000000 python_115-0.0.8.7/PKG-INFO
```

### Comparing `python_115-0.0.8.6.1/LICENSE` & `python_115-0.0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/cmd/check.py` & `python_115-0.0.8.7/p115/cmd/check.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/cmd/iterdir.py` & `python_115-0.0.8.7/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/cmd/qrcode.py` & `python_115-0.0.8.7/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/__init__.py` & `python_115-0.0.8.7/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/cipher.py` & `python_115-0.0.8.7/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/client.py` & `python_115-0.0.8.7/p115/component/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6811,14 +6811,427 @@
             payload = {"ac": "security_code", "type": "web", "ctype": "web", "client": "web", **payload}
         if "sign" not in payload:
             payload["sign"] = self.captcha_sign()["sign"]
         api = "https://webapi.115.com/user/captcha"
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
+    ########## Activities API ##########
+
+    @overload
+    def act_xys_get_act_info(
+        self, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_get_act_info(
+        self, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_get_act_info(
+        self, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """获取许愿树活动的信息
+        GET https://act.115.com/api/1.0/web/1.0/act2024xys/get_act_info
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/get_act_info"
+        request_kwargs.pop("parse", None)
+        return self.request(api, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_home_list(
+        self, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_home_list(
+        self, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_home_list(
+        self, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """首页的许愿树（随机刷新 15 条）
+        GET https://act.115.com/api/1.0/web/1.0/act2024xys/home_list
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/home_list"
+        request_kwargs.pop("parse", None)
+        return self.request(api, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_my_desire(
+        self, 
+        payload: int | dict = 0, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_my_desire(
+        self, 
+        payload: int | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_my_desire(
+        self, 
+        payload: int | dict = 0, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """我的许愿列表
+        GET https://act.115.com/api/1.0/web/1.0/act2024xys/my_desire
+        payload:
+            - type: 0 | 1 | 2 = 0
+                # 类型
+                # - 0: 全部
+                # - 1: 进行中
+                # - 2: 已实现
+            - start: int = 0  # 开始索引
+            - page: int = 1   # 第几页
+            - limit: int = 10 # 每页大小
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/my_desire"
+        if isinstance(payload, int):
+            payload = {"start": 0, "page": 1, "limit": 10, "type": payload}
+        else:
+            payload = {"type": 0, "start": 0, "page": 1, "limit": 10, **payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_my_aid_desire(
+        self, 
+        payload: int | dict = 0, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_my_aid_desire(
+        self, 
+        payload: int | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_my_aid_desire(
+        self, 
+        payload: int | dict = 0, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """我的助愿列表
+        GET https://act.115.com/api/1.0/web/1.0/act2024xys/my_aid_desire
+        payload:
+            - type: 0 | 1 | 2 = 0
+                # 类型
+                # - 0: 全部
+                # - 1: 进行中
+                # - 2: 已实现
+            - start: int = 0  # 开始索引
+            - page: int = 1   # 第几页
+            - limit: int = 10 # 每页大小
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/my_aid_desire"
+        if isinstance(payload, int):
+            payload = {"start": 0, "page": 1, "limit": 10, "type": payload}
+        else:
+            payload = {"type": 0, "start": 0, "page": 1, "limit": 10, **payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_wish(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_wish(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_wish(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """创建许愿
+        POST https://act.115.com/api/1.0/web/1.0/act2024xys/wish
+        payload:
+            - content: str # 许愿文本，不少于 5 个字，不超过 500 个字
+            - rewardSpace: int = 5 # 奖励容量，单位是 GB
+            - images: int | str = <default> # 图片文件在你的网盘的 id，多个用逗号 "," 隔开
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/wish"
+        if isinstance(payload, str):
+            payload = {"rewardSpace": 5, "content": payload}
+        else:
+            payload = {"rewardSpace": 5, **payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_wish_del(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_wish_del(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_wish_del(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """删除许愿
+        POST https://act.115.com/api/1.0/web/1.0/act2024xys/del_wish
+        payload:
+            - ids: str # 许愿的 id，多个用逗号 "," 隔开
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/del_wish"
+        if isinstance(payload, str):
+            payload = {"ids": payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_aid_desire(
+        self, 
+        payload: dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_aid_desire(
+        self, 
+        payload: dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_aid_desire(
+        self, 
+        payload: dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """创建助愿（如果提供 file_ids，则会创建一个分享链接）
+        POST https://act.115.com/api/1.0/web/1.0/act2024xys/aid_desire
+        payload:
+            - id: str # 许愿 id
+            - content: str # 助愿文本，不少于 5 个字，不超过 500 个字
+            - images: int | str = <default> # 图片文件在你的网盘的 id，多个用逗号 "," 隔开
+            - file_ids: int | str = <default> # 文件在你的网盘的 id，多个用逗号 "," 隔开
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/aid_desire"
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_aid_desire_del(
+        self, 
+        payload: int | str | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_aid_desire_del(
+        self, 
+        payload: int | str | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_aid_desire_del(
+        self, 
+        payload: int | str | dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """删除助愿
+        POST https://act.115.com/api/1.0/web/1.0/act2024xys/del_aid_desire
+        payload:
+            - ids: int | str # 助愿的 id，多个用逗号 "," 隔开
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/del_aid_desire"
+        if isinstance(payload, (int, str)):
+            payload = {"ids": payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", params=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_get_desire_info(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_get_desire_info(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_get_desire_info(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """获取的许愿信息
+        GET https://act.115.com/api/1.0/web/1.0/act2024xys/get_desire_info
+        payload:
+            - id: str # 许愿的 id
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/get_desire_info"
+        if isinstance(payload, str):
+            payload = {"id": payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_desire_aid_list(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_desire_aid_list(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_desire_aid_list(
+        self, 
+        payload: str | dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """获取许愿的助愿列表
+        GET https://act.115.com/api/1.0/web/1.0/act2024xys/desire_aid_list
+        payload:
+            - id: str         # 许愿的 id
+            - start: int = 0  # 开始索引
+            - page: int = 1   # 第几页
+            - limit: int = 10 # 每页大小
+            - sort: int | str = <default>
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/desire_aid_list"
+        if isinstance(payload, str):
+            payload = {"start": 0, "page": 1, "limit": 10, "id": payload}
+        else:
+            payload = {"start": 0, "page": 1, "limit": 10, **payload}
+        request_kwargs.pop("parse", None)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
+
+    @overload
+    def act_xys_adopt(
+        self, 
+        payload: dict, 
+        /,
+        async_: Literal[False] = False, 
+        **request_kwargs, 
+    ) -> dict:
+        ...
+    @overload
+    def act_xys_adopt(
+        self, 
+        payload: dict, 
+        /,
+        async_: Literal[True], 
+        **request_kwargs, 
+    ) -> Awaitable[dict]:
+        ...
+    def act_xys_adopt(
+        self, 
+        payload: dict, 
+        /,
+        async_: Literal[False, True] = False, 
+        **request_kwargs, 
+    ) -> dict | Awaitable[dict]:
+        """采纳助愿
+        POST https://act.115.com/api/1.0/web/1.0/act2024xys/adopt
+        payload:
+            - did: str # 许愿的 id
+            - aid: int | str # 助愿的 id
+            - to_cid: int = <default> # 助愿中的分享链接转存到你的网盘中目录的 id
+        """
+        api = "https://act.115.com/api/1.0/web/1.0/act2024xys/adopt"
+        request_kwargs.pop("parse", None)
+        return self.request(api, "POST", params=payload, async_=async_, **request_kwargs)
+
     ########## Other Encapsulations ##########
 
     # TODO 支持异步
     @overload
     def open(
         self, 
         /,
```

### Comparing `python_115-0.0.8.6.1/p115/component/fs.py` & `python_115-0.0.8.7/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/fs_base.py` & `python_115-0.0.8.7/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/fs_share.py` & `python_115-0.0.8.7/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/fs_zip.py` & `python_115-0.0.8.7/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/labellist.py` & `python_115-0.0.8.7/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/offline.py` & `python_115-0.0.8.7/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/recyclebin.py` & `python_115-0.0.8.7/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/p115/component/sharing.py` & `python_115-0.0.8.7/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/pyproject.toml` & `python_115-0.0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.6.1"
+version = "0.0.8.7"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.6.1/readme.md` & `python_115-0.0.8.7/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.6.1/PKG-INFO` & `python_115-0.0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.6.1
+Version: 0.0.8.7
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

