# Comparing `tmp/nonebot_plugin_aising-0.1.0.tar.gz` & `tmp/nonebot_plugin_aising-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_aising-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_aising-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_aising-0.1.0.tar` & `nonebot_plugin_aising-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2024-05-29 10:21:25.319362 nonebot_plugin_aising-0.1.0/LICENSE
--rw-r--r--   0        0        0     3150 2024-05-29 10:21:25.319362 nonebot_plugin_aising-0.1.0/README.md
--rw-r--r--   0        0        0     6716 2024-05-29 10:21:25.319362 nonebot_plugin_aising-0.1.0/nonebot_plugin_aising/__init__.py
--rw-r--r--   0        0        0      525 2024-05-29 10:21:25.319362 nonebot_plugin_aising-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 nonebot_plugin_aising-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-29 12:07:19.645362 nonebot_plugin_aising-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3150 2024-05-29 12:07:19.645362 nonebot_plugin_aising-0.1.1/README.md
+-rw-r--r--   0        0        0     6716 2024-05-29 12:07:19.645362 nonebot_plugin_aising-0.1.1/nonebot_plugin_aising/__init__.py
+-rw-r--r--   0        0        0      563 2024-05-29 12:07:19.645362 nonebot_plugin_aising-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 nonebot_plugin_aising-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_aising-0.1.0/LICENSE` & `nonebot_plugin_aising-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aising-0.1.0/README.md` & `nonebot_plugin_aising-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aising-0.1.0/nonebot_plugin_aising/__init__.py` & `nonebot_plugin_aising-0.1.1/nonebot_plugin_aising/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_aising-0.1.0/pyproject.toml` & `nonebot_plugin_aising-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "nonebot-plugin-aising"
-version = "0.1.0"
+version = "0.1.1"
 description = "能让b站任何能搜到素材的角色唱歌"
-authors = ["CCYellowStar"]
+authors = ["CCYellowStar","syagina"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/CCYellowStar2/nonebot-plugin-aising"
 repository = "https://github.com/CCYellowStar2/nonebot-plugin-aising"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4"
-nonebot2 = ">=2.0.0-beta.1"
+python = ">=3.9,<4"
+nonebot2 = ">=2.2.1"
 gradio_client = "^0.16.4"
+nonebot-adapter-onebot = ">=2.2.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_aising-0.1.0/PKG-INFO` & `nonebot_plugin_aising-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-aising
-Version: 0.1.0
+Version: 0.1.1
 Summary: 能让b站任何能搜到素材的角色唱歌
 Home-page: https://github.com/CCYellowStar2/nonebot-plugin-aising
 License: GPL-3.0-only
 Author: CCYellowStar
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: gradio_client (>=0.16.4,<0.17.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.1)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3)
+Requires-Dist: nonebot2 (>=2.2.1)
 Project-URL: Repository, https://github.com/CCYellowStar2/nonebot-plugin-aising
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-aising Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-aising Version: 0.1.1 Summary:
 è½è®©bç«ä»»ä½è½æå°ç´ æçè§è²å±æ­ Home-page: https://github.com/
 CCYellowStar2/nonebot-plugin-aising License: GPL-3.0-only Author: CCYellowStar
-Requires-Python: >=3.8,<4 Classifier: License :: OSI Approved :: GNU General
+Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: gradio_client (>=0.16.4,<0.17.0)
-Requires-Dist: nonebot2 (>=2.0.0-beta.1) Project-URL: Repository, https://
-github.com/CCYellowStar2/nonebot-plugin-aising Description-Content-Type: text/
-markdown
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: gradio_client
+(>=0.16.4,<0.17.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.3) Requires-
+Dist: nonebot2 (>=2.2.1) Project-URL: Repository, https://github.com/
+CCYellowStar2/nonebot-plugin-aising Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
   # nonebot-plugin-aising _â¨ è½è®©bç«ä»»ä½è½æå°ç´ æçè§è²å±æ­
                           â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç» ä½¿ç¨[NeuCo v2](https://www.bilibili.com/video/BV1fz42127wX/
 )ä½ä¸ºåç«¯ï¼botä½ä¸ºåç«¯è°ç¨çaiå±æ­æä»¶ï¼éè¿ç¬åbç«è§é¢åå ä¸æ¥éè®­ç»æ¥åå°åªè¦bç«ä¸æè¿ä¸ªè§è²çç´ æå°±è½è®©è¿ä¸ªè§è²å±bç«ä¸æçä»»ä½æ­ï¼æä»¶å¯ä½¿ç¨```è®¾ç½®å±æ­é¾æ¥```æ¥æå®åç«¯é¾æ¥è¾¾å°éæ¶æ´æ¢ï¼åç«¯æ­å»ºå¯ä»¥æ¬å°ä¹å¯ä»¥
 [colab](https://colab.research.google.com/drive/
```

