# Comparing `tmp/nonebot_adapter_console-0.5.0.tar.gz` & `tmp/nonebot_adapter_console-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_console-0.5.0.tar", last modified: Sat Feb 24 03:47:45 2024, max compression
+gzip compressed data, was "nonebot_adapter_console-0.6.0.tar", last modified: Thu May 30 07:26:24 2024, max compression
```

## Comparing `nonebot_adapter_console-0.5.0.tar` & `nonebot_adapter_console-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/LICENSE
--rw-r--r--   0        0        0      279 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/README.md
--rw-r--r--   0        0        0      264 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/__init__.py
--rw-r--r--   0        0        0     2122 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/adapter.py
--rw-r--r--   0        0        0     3376 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/backend.py
--rw-r--r--   0        0        0     2313 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/bot.py
--rw-r--r--   0        0        0       98 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/config.py
--rw-r--r--   0        0        0     2023 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/event.py
--rw-r--r--   0        0        0        0 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/exception.py
--rw-r--r--   0        0        0     3852 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/message.py
--rw-r--r--   0        0        0      361 2024-02-24 03:47:21.336323 nonebot_adapter_console-0.5.0/nonebot/adapters/console/utils.py
--rw-r--r--   0        0        0     1685 2024-02-24 03:47:45.440639 nonebot_adapter_console-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 nonebot_adapter_console-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/LICENSE
+-rw-r--r--   0        0        0      279 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/README.md
+-rw-r--r--   0        0        0      304 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/__init__.py
+-rw-r--r--   0        0        0     2122 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/adapter.py
+-rw-r--r--   0        0        0     3376 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/backend.py
+-rw-r--r--   0        0        0     2313 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/bot.py
+-rw-r--r--   0        0        0       98 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/config.py
+-rw-r--r--   0        0        0     2023 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/event.py
+-rw-r--r--   0        0        0        0 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/exception.py
+-rw-r--r--   0        0        0     3852 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/message.py
+-rw-r--r--   0        0        0      361 2024-05-30 07:25:56.030782 nonebot_adapter_console-0.6.0/nonebot/adapters/console/utils.py
+-rw-r--r--   0        0        0     1684 2024-05-30 07:26:24.510975 nonebot_adapter_console-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 nonebot_adapter_console-0.6.0/PKG-INFO
```

### Comparing `nonebot_adapter_console-0.5.0/LICENSE` & `nonebot_adapter_console-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.5.0/nonebot/adapters/console/adapter.py` & `nonebot_adapter_console-0.6.0/nonebot/adapters/console/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.5.0/nonebot/adapters/console/backend.py` & `nonebot_adapter_console-0.6.0/nonebot/adapters/console/backend.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.5.0/nonebot/adapters/console/bot.py` & `nonebot_adapter_console-0.6.0/nonebot/adapters/console/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.5.0/nonebot/adapters/console/event.py` & `nonebot_adapter_console-0.6.0/nonebot/adapters/console/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.5.0/nonebot/adapters/console/message.py` & `nonebot_adapter_console-0.6.0/nonebot/adapters/console/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.5.0/pyproject.toml` & `nonebot_adapter_console-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nonebot-adapter-console"
-version = "0.5.0"
+version = "0.6.0"
 description = "console adapter for nonebot2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
     { name = "MelodyKnit", email = "yanximelody@gmail.com" },
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 dependencies = [
     "nonechat<1.0.0,>=0.2.0",
     "nonebot2<3.0.0,>=2.2.0",
     "typing-extensions>=4.7.1",
     "pydantic>=1.10.0,<3.0.0,!=2.5.0,!=2.5.1",
 ]
-requires-python = ">=3.8,<4.0"
+requires-python = ">=3.9,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [tool.pdm.build]
 includes = [
     "nonebot",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "isort<5.11,>=5.10.1",
+    "isort<6.0,>=5.10.1",
     "black<25.0,>=24.0.0",
     "nonemoji<0.2,>=0.1.3",
-    "pre-commit<3.2,>=3.1.0",
-    "ruff~=0.2.0",
+    "pre-commit<4.0,>=3.1.0",
+    "ruff~=0.4.0",
 ]
 
 [tool.black]
 line-length = 88
 target-version = [
     "py38",
     "py39",
```

### Comparing `nonebot_adapter_console-0.5.0/PKG-INFO` & `nonebot_adapter_console-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-console
-Version: 0.5.0
+Version: 0.6.0
 Summary: console adapter for nonebot2
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>, MelodyKnit <yanximelody@gmail.com>, yanyongyu <yyy@nonebot.dev>
 License: MIT
-Requires-Python: <4.0,>=3.8
+Requires-Python: <4.0,>=3.9
 Requires-Dist: nonechat<1.0.0,>=0.2.0
 Requires-Dist: nonebot2<3.0.0,>=2.2.0
 Requires-Dist: typing-extensions>=4.7.1
 Requires-Dist: pydantic!=2.5.0,!=2.5.1,<3.0.0,>=1.10.0
 Description-Content-Type: text/markdown
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-console Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-console Version: 0.6.0 Summary:
 console adapter for nonebot2 Author-Email: RF-Tar-Railt
 qq.com>, MelodyKnit
 gmail.com>, yanyongyu
-nonebot.dev> License: MIT Requires-Python: <4.0,>=3.8 Requires-Dist:
+nonebot.dev> License: MIT Requires-Python: <4.0,>=3.9 Requires-Dist:
 nonechat<1.0.0,>=0.2.0 Requires-Dist: nonebot2<3.0.0,>=2.2.0 Requires-Dist:
 typing-extensions>=4.7.1 Requires-Dist: pydantic!=2.5.0,!=2.5.1,<3.0.0,>=1.10.0
 Description-Content-Type: text/markdown
                            _[_n_o_n_e_b_o_t_-_a_d_a_p_t_e_r_-_c_o_n_s_o_l_e_]
               # NoneBot-Adapter-Console _â¨ Console éé â¨_
```

