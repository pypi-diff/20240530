# Comparing `tmp/nonebot_plugin_sparkapi-1.4.1.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.4.1.tar", last modified: Tue May 28 21:49:48 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.4.2.tar", last modified: Thu May 30 06:02:44 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.4.1.tar` & `nonebot_plugin_sparkapi-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 21:49:48.329056 nonebot_plugin_sparkapi-1.4.1/
--rw-rw-rw-   0        0        0     1084 2024-05-15 03:42:49.000000 nonebot_plugin_sparkapi-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     8651 2024-05-28 21:49:48.328049 nonebot_plugin_sparkapi-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6831 2024-05-28 21:41:56.000000 nonebot_plugin_sparkapi-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 21:49:48.321083 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/
--rw-rw-rw-   0        0        0     4501 2024-05-28 21:25:44.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/ImgGenApi.py
--rw-rw-rw-   0        0        0     4002 2024-05-28 18:59:17.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/SparkApi.py
--rw-rw-rw-   0        0        0    15808 2024-05-28 21:26:03.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/__init__.py
--rw-rw-rw-   0        0        0     3919 2024-05-28 21:21:49.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/config.py
--rw-rw-rw-   0        0        0     2936 2024-05-28 19:10:10.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/funcs.py
--rw-rw-rw-   0        0        0     2949 2024-05-28 21:17:50.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/info.py
--rw-rw-rw-   0        0        0     1971 2024-05-28 21:20:50.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-28 21:49:48.328049 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/
--rw-rw-rw-   0        0        0     8651 2024-05-28 21:49:48.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2024-05-28 21:49:48.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 21:49:48.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-28 21:49:48.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-28 21:49:48.000000 nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      712 2024-05-28 21:45:24.000000 nonebot_plugin_sparkapi-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 21:49:48.329056 nonebot_plugin_sparkapi-1.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 06:02:44.761285 nonebot_plugin_sparkapi-1.4.2/
+-rw-rw-rw-   0        0        0     1084 2024-05-15 03:42:49.000000 nonebot_plugin_sparkapi-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     8947 2024-05-30 06:02:44.758776 nonebot_plugin_sparkapi-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7127 2024-05-30 05:51:26.000000 nonebot_plugin_sparkapi-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:02:44.740588 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/
+-rw-rw-rw-   0        0        0     4476 2024-05-30 01:24:46.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/ImgGenApi.py
+-rw-rw-rw-   0        0        0     2855 2024-05-30 05:42:40.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/PPTGenApi.py
+-rw-rw-rw-   0        0        0     4002 2024-05-28 18:59:17.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/SparkApi.py
+-rw-rw-rw-   0        0        0    17053 2024-05-30 05:41:43.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/__init__.py
+-rw-rw-rw-   0        0        0     4037 2024-05-30 01:34:59.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/config.py
+-rw-rw-rw-   0        0        0     2936 2024-05-28 19:10:10.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/funcs.py
+-rw-rw-rw-   0        0        0     3438 2024-05-30 05:30:35.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/info.py
+-rw-rw-rw-   0        0        0     1971 2024-05-28 21:55:39.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:02:44.753089 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/
+-rw-rw-rw-   0        0        0     8947 2024-05-30 06:02:44.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2024-05-30 06:02:44.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:02:44.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-30 06:02:44.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-30 06:02:44.000000 nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      712 2024-05-30 05:53:52.000000 nonebot_plugin_sparkapi-1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:02:44.761285 nonebot_plugin_sparkapi-1.4.2/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/LICENSE` & `nonebot_plugin_sparkapi-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.4.1/PKG-INFO` & `nonebot_plugin_sparkapi-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.4.1
+Version: 1.4.2
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,19 +67,22 @@
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
 - [x] 支持用户自定义、更改、切换预设（Prompt）
 - [x] 自动生成人物预设菜单、帮助列表，无需重写
 - [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
 - [x] 支持AI绘图（AI Image Generation）
+- [x] 支持AI生成PPT（PPT Generation）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] PPT生成（PPT Generation）
+- [ ] 用户画像（记录用户信息以便提供更精确的内容）（目前存争议，考虑允许用户自行设置）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
+- Pypi：https://pypi.org/project/nonebot-plugin-sparkapi/
+- Nonebot：https://registry.nonebot.dev/plugin/nonebot-plugin-sparkapi:nonebot_plugin_sparkapi
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -137,22 +140,22 @@
 | SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
 | SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
 | SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
 | SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
 | SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
 | SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
 | SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
-| SPARKAPI_FL_IMGGEN | 否 | True | 是否启用AI绘图功能 |
+| SPARKAPI_FL_IMGGEN | 否 | False | 是否启用AI绘图功能 |
+| SPARKAPI_FL_PPTGEN | 否 | False | 是否启用AI生成PPT功能 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
 以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
 1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
 2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
 3. sparkapi_message_blockprivate：阻断私聊时的提示信息
-4. sparkapi_message_blockimggen：阻断AI绘图时的提示信息
 
 ## 🎉 使用
 ### 指令表（默认）
 以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.4.2 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -31,19 +31,22 @@
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
 æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼Promptï¼ - [x]
 èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
 åºäºpickleçåå²è®°å½æä¹å - [x]
 å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] æ¯æAIç»å¾ï¼AI
-Image Generationï¼ - [ ]
+Image Generationï¼ - [x] æ¯æAIçæPPTï¼PPT Generationï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-PPTçæï¼PPT Generationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https://
-github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
-Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+ç¨æ·ç»åï¼è®°å½ç¨æ·ä¿¡æ¯ä»¥ä¾¿æä¾æ´ç²¾ç¡®çåå®¹ï¼ï¼ç®åå­äºè®®ï¼èèåè®¸ç¨æ·èªè¡è®¾ç½®ï¼
+### ð¦ é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-
+sparkapi - Pypiï¼https://pypi.org/project/nonebot-plugin-sparkapi/ -
+Nonebotï¼https://registry.nonebot.dev/plugin/nonebot-plugin-sparkapi:
+nonebot_plugin_sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~
+## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
 nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
 install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -75,22 +78,22 @@
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
 SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
 åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
 SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
 SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ | True
-| æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ |
+False | æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_FL_PPTGEN | å¦ | False |
+æ¯å¦å¯ç¨AIçæPPTåè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
 æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
 nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
 sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
 sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
-sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ 4.
-sparkapi_message_blockimggenï¼é»æ­AIç»å¾æ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
 ### æä»¤è¡¨ï¼é»è®¤ï¼
 ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
 ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
 | æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
 æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/README.md` & `nonebot_plugin_sparkapi-1.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,19 +31,22 @@
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
 - [x] 支持用户自定义、更改、切换预设（Prompt）
 - [x] 自动生成人物预设菜单、帮助列表，无需重写
 - [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
 - [x] 支持AI绘图（AI Image Generation）
+- [x] 支持AI生成PPT（PPT Generation）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] PPT生成（PPT Generation）
+- [ ] 用户画像（记录用户信息以便提供更精确的内容）（目前存争议，考虑允许用户自行设置）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
+- Pypi：https://pypi.org/project/nonebot-plugin-sparkapi/
+- Nonebot：https://registry.nonebot.dev/plugin/nonebot-plugin-sparkapi:nonebot_plugin_sparkapi
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -101,22 +104,22 @@
 | SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
 | SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
 | SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
 | SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
 | SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
 | SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
 | SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
-| SPARKAPI_FL_IMGGEN | 否 | True | 是否启用AI绘图功能 |
+| SPARKAPI_FL_IMGGEN | 否 | False | 是否启用AI绘图功能 |
+| SPARKAPI_FL_PPTGEN | 否 | False | 是否启用AI生成PPT功能 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
 以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
 1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
 2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
 3. sparkapi_message_blockprivate：阻断私聊时的提示信息
-4. sparkapi_message_blockimggen：阻断AI绘图时的提示信息
 
 ## 🎉 使用
 ### 指令表（默认）
 以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -9,19 +9,22 @@
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
 æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼Promptï¼ - [x]
 èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
 åºäºpickleçåå²è®°å½æä¹å - [x]
 å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] æ¯æAIç»å¾ï¼AI
-Image Generationï¼ - [ ]
+Image Generationï¼ - [x] æ¯æAIçæPPTï¼PPT Generationï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-PPTçæï¼PPT Generationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https://
-github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
-Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+ç¨æ·ç»åï¼è®°å½ç¨æ·ä¿¡æ¯ä»¥ä¾¿æä¾æ´ç²¾ç¡®çåå®¹ï¼ï¼ç®åå­äºè®®ï¼èèåè®¸ç¨æ·èªè¡è®¾ç½®ï¼
+### ð¦ é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-
+sparkapi - Pypiï¼https://pypi.org/project/nonebot-plugin-sparkapi/ -
+Nonebotï¼https://registry.nonebot.dev/plugin/nonebot-plugin-sparkapi:
+nonebot_plugin_sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~
+## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
 nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
 install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -53,22 +56,22 @@
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
 SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
 åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
 SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
 SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ | True
-| æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ |
+False | æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_FL_PPTGEN | å¦ | False |
+æ¯å¦å¯ç¨AIçæPPTåè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
 æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
 nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
 sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
 sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
-sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ 4.
-sparkapi_message_blockimggenï¼é»æ­AIç»å¾æ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
 ### æä»¤è¡¨ï¼é»è®¤ï¼
 ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
 ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
 | æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
 æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/ImgGenApi.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/ImgGenApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
     params = gen_params(appid, domain, content)
     async with httpx.AsyncClient(timeout=30.0) as client:
         print("Image Generation: Got Request, Generating...")
         st = asyncio.get_event_loop().time()
         response = await client.post(url, json=params, headers={'content-type': "application/json"})
         ed = asyncio.get_event_loop().time()
         parse_response(response.json())
-        global duration
         print(f"Time Consumed: {ed-st:.2f}s")
     return res
 
 async def main(appid, api_key, api_secret, IG_url, domain, content):
     await connect_hs(appid, api_key, api_secret, IG_url, domain, content)
     return res
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from nonebot.adapters.onebot.v11 import MessageEvent as ME,PrivateMessageEvent as PME # type: ignore
 from nonebot.adapters.onebot.v11 import Message , MessageSegment as MS # type: ignore
 
 import nonebot
 from nonebot.plugin import PluginMetadata
 from nonebot.plugin.on import on_message
 from nonebot.params import CommandArg
-from nonebot.rule import to_me,is_type,command
+from nonebot.rule import to_me,is_type
 from nonebot.params import ArgPlainText
 # from nonebot.permission import SUPERUSER
 
 from copy import deepcopy
 
-from . import SparkApi,ImgGenApi,funcs,info,storage
+from . import SparkApi,ImgGenApi,PPTGenApi,funcs,info,storage
 from .config import Config
 
 # ---------------------------Configurations---------------------------
 # 插件元数据
 __plugin_meta__ = PluginMetadata(
     name="科大讯飞星火大语言模型官方API聊天机器人插件",
     description="调用科大讯飞星火大语言模型官方API的聊天机器人插件。适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设",
@@ -42,27 +42,28 @@
 priority_function = priority_blockprivate + 1
 priority_chat = priority_blockprivate + 2
 
 commands = conf.sparkapi_commands
 fl_group_at = conf.sparkapi_fl_group_at
 fl_notice = conf.sparkapi_fl_notice
 fl_setpreset_clear = conf.sparkapi_fl_setpreset_clear
-fl_imggen = conf.sparkapi_fl_imggen
 maxlength = conf.sparkpai_model_maxlength
 priority = conf.sparkapi_priority
 
 sessions = {} # 会话记录
 spname = {} # 选取的prompt
 presets = {} # 人物预设列表
 
 # if not appid or not api_secret or not api_key:
 #     raise ConfigError("请设置API信息,可前往 https://console.xfyun.cn/ 获取")
 
 # ---------------------------Tests---------------------------
 
+
+
 # ---------------------------Matchers---------------------------
 # 事件响应器：私聊阻断
 async def fl_blockprivate() -> bool:
     return not conf.sparkapi_fl_private_chat
 rule_blockprivate = is_type(PME) & fl_blockprivate
 matcher_blockprivate = on_message(
     rule = rule_blockprivate,
@@ -375,26 +376,25 @@
         spname[session_id] = pname
         await matcher_session_load.finish(MS.text("已加载上次保存的对话记录！"))
     else:
         await matcher_session_load.finish(MS.text("未保存对话记录"))
 
 
 # 事件响应器：AI绘图
-rule_imggen = to_me() & funcs.trans_command(commands["image_generation"])
+async def fl_imggen() -> bool:
+    return conf.sparkapi_fl_imggen
+rule_imggen = to_me() & funcs.trans_command(commands["image_generation"]) & fl_imggen
 matcher_imggen = on_message(
     rule = rule_imggen,
     priority = priority_function,
     block = True
 )
 
 @matcher_imggen.handle()
 async def imggen_handle_function(event: ME, msg: Message = CommandArg()):
-    if not fl_imggen:
-        await matcher_imggen.finish(MS.text(conf.sparkapi_message_blockimggen))
-    
     content = msg.extract_plain_text().strip()
     session_id = funcs.get_session_id(event)
 
     if content : 
         if len(content) > maxlength:
             await matcher_imggen.finish(MS.text(f"输入文字过长：请不要超过{maxlength}字节！"))
         ret = await request_IG(content)
@@ -411,14 +411,44 @@
     session_id = funcs.get_session_id(event)
 
     ret = await request_IG(content)
     path = storage.f_image_base64_save(ret, f"{session_id}.png")
     await matcher_imggen.finish(MS.image(path))
 
 
+# 事件响应器：AI生成PPT
+async def fl_pptgen() -> bool:
+    return conf.sparkapi_fl_pptgen
+rule_pptgen = to_me() & funcs.trans_command(commands["ppt_generation"]) & fl_pptgen
+matcher_pptgen = on_message(
+    rule = rule_pptgen,
+    priority = priority_function,
+    block = True
+)
+
+@matcher_pptgen.handle()
+async def pptgen_handle_function(event: ME, msg: Message = CommandArg()):
+    content = msg.extract_plain_text().strip()
+    
+    if content:
+        if len(content) > maxlength:
+            await matcher_pptgen.finish(MS.text(f"输入文字过长：请不要超过{maxlength}字节！"))
+        ret = await request_IP(content)
+        await matcher_pptgen.finish(MS.text("点击链接下载："+ret))
+        
+@matcher_pptgen.got("content",prompt="请输入文字描述\n回复“取消”退出")
+async def pptgen_got_function(event: ME, content: str = ArgPlainText()):
+    if content=="取消":
+        await matcher_pptgen.finish(MS.text("操作已取消"))
+    if len(content) > maxlength:
+        await matcher_pptgen.finish(MS.text(f"输入文字过长：请不要超过{maxlength}字节！"))
+    
+    ret = await request_IP(content)
+    await matcher_pptgen.finish(MS.text("点击链接下载："+ret))
+
 # ---------------------------API Request---------------------------
 model_version = funcs.unify_model_version(conf.sparkapi_model_version)
 Spark_url = funcs.get_Spark_url(model_version)
 domain = funcs.get_domain(model_version)
 
 async def request(history, sid, session_id, pname):
     history = deepcopy(history)
@@ -430,10 +460,13 @@
     return SparkApi.answer
 
 IG_url = "http://spark-api.cn-huabei-1.xf-yun.com/v2.1/tti"
 IG_domain = "general"
 
 async def request_IG(content):
     ImgGenApi.res = ""
-    ImgGenApi.duration = 0
     await ImgGenApi.main(appid,api_key,api_secret,IG_url,IG_domain,content)
     return ImgGenApi.res
+
+async def request_IP(content):
+    res = await PPTGenApi.main(appid, api_secret, content)
+    return res
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,39 +25,41 @@
         "preset_set" : ["set","切换预设"], # 切换人物预设
         "preset_create" : ["create","创建预设"], # 创建人物预设
         "preset_delete" : ["delete","删除预设"], # 删除人物预设
         "session_clear" : ["clear","清空对话"], # 清空对话
         "session_save" : ["save","保存对话"], # 保存对话记录
         "session_load" : ["load","加载对话"],  # 加载对话记录
         "image_generation" : ["imggen","AI绘图"],  # AI绘图
+        "ppt_generation" : ["pptgen","AIPPT",],  # AI制作PPT
     }
     sparkapi_commands_info: dict[str, str] = { # 命令说明，用于生成帮助信息
         "chat" : "与机器人进行对话",
         "help" : "显示帮助信息",
         "preset_show" : "显示人物预设菜单和当前预设",
         "preset_set" : "切换人物预设",
         "preset_create" : "创建人物预设",
         "preset_delete" : "删除人物预设",
         "session_clear" : "清空当前对话上下文",
         "session_save" : "保存本次对话记录",
         "session_load" : "加载上次保存的对话记录",
         "image_generation" : "AI根据文字描述绘制一张图片",
+        "ppt_generation" : "AI根据文字描述制作PPT",
     }
 
     # 聊天设置
-    sparkapi_fl_notice: bool = True # 收到请求时是否提示已收到请求
+    sparkapi_fl_notice: bool = False # 收到请求时是否提示已收到请求
     sparkapi_fl_setpreset_clear: bool = True # 切换人物预设时是否清空上下文
 
     # 私聊设置
     sparkapi_fl_private_chat: bool = True # 允许私聊
     sparkapi_message_blockprivate: str = "私聊功能已关闭！如有需要，请联系管理员。" # 阻断私聊时的提示信息
     
     # 群聊设置
     sparkapi_fl_group_public: bool = False # 群聊启用公共会话：True：所有人共享同一会话；False：每个人的会话各自独立
     sparkapi_fl_group_at: bool = True # 群聊中，回复时是否需要@提问者
     
-    # 图片生成功能，API信息一般与AI对话API一致
-    sparkapi_fl_imggen : bool = True # 启用图片生成功能
-    sparkapi_message_blockimggen : str = "图片生成功能已关闭！如有需要，请联系管理员。" # 阻断图片生成功能时的提示信息
+    # 扩展功能
+    sparkapi_fl_imggen : bool = False # 启用图片生成功能，需要申请独立用量，API信息一般与AI对话API一致
+    sparkapi_fl_pptgen : bool = False # 启用PPT生成功能，需要申请独立用量，API信息一般与AI对话API一致
 
     # 机器人名字
     sparkapi_bot_name: str = "" # 机器人名字
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/info.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/info.py`

 * *Files 25% similar despite different names*

```diff
@@ -51,17 +51,34 @@
 presets_lst_default = get_preset_lst(presets_default,{})
 
 # 生成帮助信息
 def get_help_info(commands:dict,commands_info:dict)->str:
     def unify_command(command_info:list)->str:
         ret = "/".join(command_info)
         return ret
+    
     help_info = "【帮助信息】\n"
     command_chat = unify_command(commands["chat"])
-    help_info += f"1. {command_chat+'+' if command_chat else '直接发送'}对话内容：与机器人进行对话\n"
-    for i, (command, command_info) in enumerate(commands_info.items(), start=1):
-        if command == "chat":
+    help_info += f"1. {command_chat+'+' if command_chat else '直接发送'}对话内容：{commands_info['chat']}\n"
+    i = 2
+    special_commands = ["chat", "image_generation", "ppt_generation"]
+
+    for command, command_info in commands_info.items():
+        if command in special_commands:
             continue
         command = unify_command(commands[command])
         help_info += f"{i}. {command}：{command_info}\n"
+        i += 1
+
+    if conf.sparkapi_fl_imggen:
+        command_imggen = unify_command(commands["image_generation"])
+        help_info += f"{i}. {command_imggen}：{commands_info['image_generation']}\n"
+        i += 1
+
+    if conf.sparkapi_fl_pptgen:
+        command_pptgen = unify_command(commands["ppt_generation"])
+        help_info += f"{i}. {command_pptgen}：{commands_info['ppt_generation']}\n"
+        i += 1
+
     return help_info
+
 help_info = get_help_info(commands,commands_info)
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi/storage.py` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi/storage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.4.1/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.4.2/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.4.1
+Version: 1.4.2
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -67,19 +67,22 @@
 - [x] 支持上下文关联记忆（可设置记忆文本长度）
 - [x] 用户鉴别（每个用户的历史记录独立）
 - [x] 支持用户自定义、更改、切换预设（Prompt）
 - [x] 自动生成人物预设菜单、帮助列表，无需重写
 - [x] 基于pickle的历史记录持久化
 - [x] 完善的配置项（有其他需求请发issue）
 - [x] 支持AI绘图（AI Image Generation）
+- [x] 支持AI生成PPT（PPT Generation）
 - [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] PPT生成（PPT Generation）
+- [ ] 用户画像（记录用户信息以便提供更精确的内容）（目前存争议，考虑允许用户自行设置）
 
 ### 📦 项目地址
 - Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
+- Pypi：https://pypi.org/project/nonebot-plugin-sparkapi/
+- Nonebot：https://registry.nonebot.dev/plugin/nonebot-plugin-sparkapi:nonebot_plugin_sparkapi
 - 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
 
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
@@ -137,22 +140,22 @@
 | SPARKAPI_PRIORITY | 否 | 80 | 该值越小，事件越先被触发。本插件建议设置较大的值。可选值：1~97<br>若触发本插件事件，所有插件中优先级大于此值的事件都将被阻断。<br>本插件中事件的优先级顺序：私聊阻断（=priority）< 功能（=priority+1）< 对话（=priority+2） |
 | SPARKAPI_COMMANDS__CHAT | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空：COMMAND_START = [""]） |
 | SPARKAPI_FL_NOTICE | 否 | True | 收到请求时是否提示“已收到请求” |
 | SPARKAPI_FL_SETPRESET_CLEAR | 否 | True | 切换人物预设时是否清除当前对话上下文 |
 | SPARKAPI_FL_PRIVATE_CHAT | 否 | True | 是否允许私聊使用 |
 | SPARKAPI_FL_GROUP_PUBLIC | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
 | SPARKAPI_FL_GROUP_AT | 否 | True | 群聊回复消息时是否需要@提问者 |
-| SPARKAPI_FL_IMGGEN | 否 | True | 是否启用AI绘图功能 |
+| SPARKAPI_FL_IMGGEN | 否 | False | 是否启用AI绘图功能 |
+| SPARKAPI_FL_PPTGEN | 否 | False | 是否启用AI生成PPT功能 |
 | SPARKAPI_BOT_NAME | 否 | "" | 机器人的名字 |
 
 以下配置项请查看`/.venv/Lib/nonebot_plugin_sparkapi/config.py`修改：
 1. sparkapi_commands：指令表（允许单个字符串或字符串列表）
 2. sparkapi_commands_info：指令表说明（用于生成帮助信息）
 3. sparkapi_message_blockprivate：阻断私聊时的提示信息
-4. sparkapi_message_blockimggen：阻断AI绘图时的提示信息
 
 ## 🎉 使用
 ### 指令表（默认）
 以下所有指令均可在config.py中修改，且无需重写菜单/指令生成函数
 
 | 指令 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.4.2 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -31,19 +31,22 @@
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
 æ¯æç¨æ·èªå®ä¹ãæ´æ¹ãåæ¢é¢è®¾ï¼Promptï¼ - [x]
 èªå¨çæäººç©é¢è®¾èåãå¸®å©åè¡¨ï¼æ ééå - [x]
 åºäºpickleçåå²è®°å½æä¹å - [x]
 å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] æ¯æAIç»å¾ï¼AI
-Image Generationï¼ - [ ]
+Image Generationï¼ - [x] æ¯æAIçæPPTï¼PPT Generationï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-PPTçæï¼PPT Generationï¼ ### ð¦ é¡¹ç®å°å - Githubï¼https://
-github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
-Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+ç¨æ·ç»åï¼è®°å½ç¨æ·ä¿¡æ¯ä»¥ä¾¿æä¾æ´ç²¾ç¡®çåå®¹ï¼ï¼ç®åå­äºè®®ï¼èèåè®¸ç¨æ·èªè¡è®¾ç½®ï¼
+### ð¦ é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-
+sparkapi - Pypiï¼https://pypi.org/project/nonebot-plugin-sparkapi/ -
+Nonebotï¼https://registry.nonebot.dev/plugin/nonebot-plugin-sparkapi:
+nonebot_plugin_sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~
+## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
 è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
 nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
 install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
@@ -75,22 +78,22 @@
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | |
 SPARKAPI_FL_SETPRESET_CLEAR | å¦ | True |
 åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | |
 SPARKAPI_FL_PRIVATE_CHAT | å¦ | True | æ¯å¦åè®¸ç§èä½¿ç¨ | |
 SPARKAPI_FL_GROUP_PUBLIC | å¦ | False | ç¾¤èå¯ç¨å¬å±ä¼è¯
 Trueï¼ææäººå±äº«åä¸ä¼è¯
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | SPARKAPI_FL_GROUP_AT | å¦ | True |
-ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ | True
-| æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
+ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | SPARKAPI_FL_IMGGEN | å¦ |
+False | æ¯å¦å¯ç¨AIç»å¾åè½ | | SPARKAPI_FL_PPTGEN | å¦ | False |
+æ¯å¦å¯ç¨AIçæPPTåè½ | | SPARKAPI_BOT_NAME | å¦ | "" |
 æºå¨äººçåå­ | ä»¥ä¸éç½®é¡¹è¯·æ¥ç`/.venv/Lib/
 nonebot_plugin_sparkapi/config.py`ä¿®æ¹ï¼ 1.
 sparkapi_commandsï¼æä»¤è¡¨ï¼åè®¸åä¸ªå­ç¬¦ä¸²æå­ç¬¦ä¸²åè¡¨ï¼ 2.
 sparkapi_commands_infoï¼æä»¤è¡¨è¯´æï¼ç¨äºçæå¸®å©ä¿¡æ¯ï¼ 3.
-sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ 4.
-sparkapi_message_blockimggenï¼é»æ­AIç»å¾æ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
+sparkapi_message_blockprivateï¼é»æ­ç§èæ¶çæç¤ºä¿¡æ¯ ## ð ä½¿ç¨
 ### æä»¤è¡¨ï¼é»è®¤ï¼
 ä»¥ä¸æææä»¤åå¯å¨config.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
 æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
 -:|:----:| | SPARKAPI_COMMAND_CHATï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
 ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help/å¸®å© | æ¯ | ç§è/ç¾¤è
 | æ¾ç¤ºå¸®å©ä¿¡æ¯ | | preset/äººç©é¢è®¾ | æ¯ | ç§è/ç¾¤è |
 æ¾ç¤ºäººç©é¢è®¾èååå½åé¢è®¾ | | set/åæ¢é¢è®¾ | æ¯ | ç§è/
```

### Comparing `nonebot_plugin_sparkapi-1.4.1/pyproject.toml` & `nonebot_plugin_sparkapi-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.4.1"
+version = "1.4.2"
 description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
     "nonebot2 >=2.0.0rc3, <3.0.0",
```

