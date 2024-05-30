# Comparing `tmp/anotify-0.1.0.tar.gz` & `tmp/anotify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.1.0.tar", last modified: Fri May 10 13:31:42 2024, max compression
+gzip compressed data, was "anotify-0.1.1.tar", last modified: Thu May 30 02:27:52 2024, max compression
```

## Comparing `anotify-0.1.0.tar` & `anotify-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:42.820253 anotify-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:42.820253 anotify-0.1.0/ANotify/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Nanpush.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Ndingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Nemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Nfeishu.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Niyuu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Npushplus.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Nserverchan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Ntelegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/Nwecom.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 13:31:38.000000 anotify-0.1.0/ANotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 13:31:38.000000 anotify-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-10 13:31:42.820253 anotify-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-10 13:31:38.000000 anotify-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:31:42.820253 anotify-0.1.0/anotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-10 13:31:42.000000 anotify-0.1.0/anotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-10 13:31:42.000000 anotify-0.1.0/anotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:31:42.000000 anotify-0.1.0/anotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 13:31:42.000000 anotify-0.1.0/anotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 13:31:42.000000 anotify-0.1.0/anotify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:31:42.820253 anotify-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 13:31:38.000000 anotify-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:27:52.559372 anotify-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:27:52.555372 anotify-0.1.1/ANotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nanpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Ndingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nfeishu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Niyuu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Npushplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nserverchan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Ntelegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/Nwecom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-30 02:27:45.000000 anotify-0.1.1/ANotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 02:27:45.000000 anotify-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-30 02:27:52.559372 anotify-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-30 02:27:45.000000 anotify-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:27:52.559372 anotify-0.1.1/anotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 02:27:52.000000 anotify-0.1.1/anotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:27:52.559372 anotify-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-30 02:27:45.000000 anotify-0.1.1/setup.py
```

### Comparing `anotify-0.1.0/ANotify/Nanpush.py` & `anotify-0.1.1/ANotify/Nanpush.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Ndingtalk.py` & `anotify-0.1.1/ANotify/Ndingtalk.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Nemail.py` & `anotify-0.1.1/ANotify/Nemail.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Nfeishu.py` & `anotify-0.1.1/ANotify/Nfeishu.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Npushplus.py` & `anotify-0.1.1/ANotify/Npushplus.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Nserverchan.py` & `anotify-0.1.1/ANotify/Nserverchan.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Ntelegram.py` & `anotify-0.1.1/ANotify/Ntelegram.py`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/ANotify/Nwecom.py` & `anotify-0.1.1/ANotify/Nwecom.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,33 @@
             "enable_duplicate_check": 0,
             "duplicate_check_interval": 1800
         }
         resp = requests.post(url, data=json.dumps(payload))
         resp.raise_for_status()
         return resp.json()
 
+    # 发送 Markdown 消息
+    def send_msg_mardown(self, text):
+        url = 'https://qyapi.weixin.qq.com/cgi-bin/message/send?access_token=' + self.access_token
+        payload = {
+            "touser": "@all",
+            "msgtype": "markdown",
+            "agentid": self.agentid,
+            "text": {
+                "content": text
+            },
+            "safe": 0,
+            "enable_id_trans": 0,
+            "enable_duplicate_check": 0,
+            "duplicate_check_interval": 1800
+        }
+        resp = requests.post(url, data=json.dumps(payload))
+        resp.raise_for_status()
+        return resp.json()
+
     # 发送图片消息
     def send_img(self, img_path):
         url = 'https://qyapi.weixin.qq.com/cgi-bin/message/send?access_token=' + self.access_token
         payload = {
             "touser": "@all",
             "msgtype": "image",
             "agentid": self.agentid,
```

### Comparing `anotify-0.1.0/LICENSE` & `anotify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.1.0/PKG-INFO` & `anotify-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.1.0
+Version: 0.1.1
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
 # 应用Secret
 CORPSECRET = ''
 # 应用ID
 AgentId = ''
 
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
+wn.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
 
 # Webhook
 WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx"
 wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
@@ -74,16 +75,15 @@
 feishu.send_file(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "test.txt")
 
 # Webhook
 feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx")
 feishu_webhook.send_msg("Hello World!")
 ```
 
-### 飞书
-[官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
+### 钉钉 
 [Webhook请求发送消息](https://open.dingtalk.com/document/robots/custom-robot-access)
 ```python
 from ANotify import Ndingtalk
 
 WEB_HOOK = "https://oapi.dingtalk.com/robot/send?access_token=xxxxxx"
 dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify(WEB_HOOK)
 dingtalk_webhook.send_msg("Hello World!")
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.1.0 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.1.1 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
 å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/)
 [ç¾¤èæºå¨äººWebhook](https://open.work.weixin.qq.com/help2/pc/14931)
 ```python from ANotify import Nwecom # ä¼ä¸ID CORPID = '' # åºç¨Secret
 CORPSECRET = '' # åºç¨ID AgentId = '' wn = Nwecom.WxNotify(corpid=CORPID,
 corpsecret=CORPSECRET, agentid=AgentId) wn.send_msg("test message")
-wn.send_text_card("test title", "test content", "https://www.example.com")
-wn.send_file("./test.txt") wn.send_img("./test.png") # Webhook WEB_HOOK =
-"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx" wn_webhook =
-Nwecom.WxWebhookNotify(WEB_HOOK) wn_webhook.send_msg("Hello")
-wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://
-github.com/TommyMerlin/ANotify)") wn_webhook.send_img("E:/Desktop/gpt/
-Cursor_Demo/test.png") wn_webhook.send_file("test.png") ``` ### é£ä¹¦ [å®ç½]
-(https://open.feishu.cn/document/server-docs/im-v1/introduction) [åå»ºåºç¨]
-(https://open.feishu.cn/document/home/introduction-to-custom-app-development/
-self-built-application-development-process) [APIè°è¯å°](https://
-open.feishu.cn/api-explorer?from=op_doc_tab) [è·åæ¶æ¯åéå¯¹è±¡ openid]
-(https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
-[Webhookè¯·æ±åéæ¶æ¯](https://open.feishu.cn/document/client-docs/bot-v3/
-add-custom-bot#355ec8c0) ```python from ANotify import Nfeishu APPID = ''
-APPSECRET = '' OPEN_ID = '' UNION_ID = '' USER_ID = '' CHAT_ID = '' feishu =
-Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET) feishu.send_msg
-(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!") feishu.send_msg
-(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!") feishu.send_msg
-(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!") feishu.send_msg
-(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!") # åéå¾ç
-feishu.send_img(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "test.png") #
-åéæä»¶ feishu.send_file(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
-"test.txt") # Webhook feishu_webhook = Nfeishu.FeishuWebhookNotify("https://
-open.feishu.cn/open-apis/bot/v2/hook/xxxxxx") feishu_webhook.send_msg("Hello
-World!") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-docs/
-im-v1/introduction) [Webhookè¯·æ±åéæ¶æ¯](https://open.dingtalk.com/
-document/robots/custom-robot-access) ```python from ANotify import Ndingtalk
-WEB_HOOK = "https://oapi.dingtalk.com/robot/send?access_token=xxxxxx"
-dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify(WEB_HOOK)
-dingtalk_webhook.send_msg("Hello World!") ``` ### AnPush [å®ç½](https://
-anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
+wn.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/
+TommyMerlin/ANotify)") wn.send_text_card("test title", "test content", "https:/
+/www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png") #
+Webhook WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/
+send?key=xxxxxx" wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn_webhook.send_msg("Hello") wn_webhook.send_msg_markdown("**Hello**\n-
+test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
+wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png") wn_webhook.send_file
+("test.png") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-
+docs/im-v1/introduction) [åå»ºåºç¨](https://open.feishu.cn/document/home/
+introduction-to-custom-app-development/self-built-application-development-
+process) [APIè°è¯å°](https://open.feishu.cn/api-explorer?from=op_doc_tab)
+[è·åæ¶æ¯åéå¯¹è±¡ openid](https://open.feishu.cn/document/faq/trouble-
+shooting/how-to-obtain-openid) [Webhookè¯·æ±åéæ¶æ¯](https://
+open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0) ```python
+from ANotify import Nfeishu APPID = '' APPSECRET = '' OPEN_ID = '' UNION_ID =
+'' USER_ID = '' CHAT_ID = '' feishu = Nfeishu.FeishuNotify(appid=APPID,
+appsecret=APPSECRET) feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
+"Hello World!") feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID,
+"Hello World!") feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello
+World!") feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
+# åéå¾ç feishu.send_img(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
+"test.png") # åéæä»¶ feishu.send_file(Nfeishu.ReceiverType.OPEN_ID,
+OPEN_ID, "test.txt") # Webhook feishu_webhook = Nfeishu.FeishuWebhookNotify
+("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx") feishu_webhook.send_msg
+("Hello World!") ``` ### éé [Webhookè¯·æ±åéæ¶æ¯](https://
+open.dingtalk.com/document/robots/custom-robot-access) ```python from ANotify
+import Ndingtalk WEB_HOOK = "https://oapi.dingtalk.com/robot/
+send?access_token=xxxxxx" dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify
+(WEB_HOOK) dingtalk_webhook.send_msg("Hello World!") ``` ### AnPush [å®ç½]
+(https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
 Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
 ``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
 TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ```
 ### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from ANotify import
 NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus =
 Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯æ­£æ", Npushplus.TemplateType.txt) msg_json = { "status": 200, "msg":
```

### Comparing `anotify-0.1.0/README.md` & `anotify-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # 应用Secret
 CORPSECRET = ''
 # 应用ID
 AgentId = ''
 
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
+wn.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
 
 # Webhook
 WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx"
 wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
@@ -59,16 +60,15 @@
 feishu.send_file(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "test.txt")
 
 # Webhook
 feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx")
 feishu_webhook.send_msg("Hello World!")
 ```
 
-### 飞书
-[官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
+### 钉钉 
 [Webhook请求发送消息](https://open.dingtalk.com/document/robots/custom-robot-access)
 ```python
 from ANotify import Ndingtalk
 
 WEB_HOOK = "https://oapi.dingtalk.com/robot/send?access_token=xxxxxx"
 dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify(WEB_HOOK)
 dingtalk_webhook.send_msg("Hello World!")
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
 ![Alt](https://repobeats.axiom.co/api/embed/
 e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image") ##
 å®è£ ```console pip install anotify ``` ## å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½]
 (https://work.weixin.qq.com/) [ç¾¤èæºå¨äººWebhook](https://
 open.work.weixin.qq.com/help2/pc/14931) ```python from ANotify import Nwecom #
 ä¼ä¸ID CORPID = '' # åºç¨Secret CORPSECRET = '' # åºç¨ID AgentId = '' wn
 = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
-wn.send_msg("test message") wn.send_text_card("test title", "test content",
-"https://www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png")
-# Webhook WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/
-send?key=xxxxxx" wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn.send_msg("test message") wn.send_msg_markdown("**Hello**\n- test1\n-
+[ANotify](https://github.com/TommyMerlin/ANotify)") wn.send_text_card("test
+title", "test content", "https://www.example.com") wn.send_file("./test.txt")
+wn.send_img("./test.png") # Webhook WEB_HOOK = "https://qyapi.weixin.qq.com/
+cgi-bin/webhook/send?key=xxxxxx" wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
 wn_webhook.send_msg("Hello") wn_webhook.send_msg_markdown("**Hello**\n-
 test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
 wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png") wn_webhook.send_file
 ("test.png") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-
 docs/im-v1/introduction) [åå»ºåºç¨](https://open.feishu.cn/document/home/
 introduction-to-custom-app-development/self-built-application-development-
 process) [APIè°è¯å°](https://open.feishu.cn/api-explorer?from=op_doc_tab)
@@ -25,16 +26,15 @@
 "Hello World!") feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID,
 "Hello World!") feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello
 World!") feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
 # åéå¾ç feishu.send_img(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
 "test.png") # åéæä»¶ feishu.send_file(Nfeishu.ReceiverType.OPEN_ID,
 OPEN_ID, "test.txt") # Webhook feishu_webhook = Nfeishu.FeishuWebhookNotify
 ("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx") feishu_webhook.send_msg
-("Hello World!") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/
-server-docs/im-v1/introduction) [Webhookè¯·æ±åéæ¶æ¯](https://
+("Hello World!") ``` ### éé [Webhookè¯·æ±åéæ¶æ¯](https://
 open.dingtalk.com/document/robots/custom-robot-access) ```python from ANotify
 import Ndingtalk WEB_HOOK = "https://oapi.dingtalk.com/robot/
 send?access_token=xxxxxx" dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify
 (WEB_HOOK) dingtalk_webhook.send_msg("Hello World!") ``` ### AnPush [å®ç½]
 (https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
 Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
 ``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
```

### Comparing `anotify-0.1.0/anotify.egg-info/PKG-INFO` & `anotify-0.1.1/anotify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anotify
-Version: 0.1.0
+Version: 0.1.1
 Summary: Send notifications by multiple channels.
 Home-page: https://github.com/TommyMerlin/ANotify
 Author: 7ommy
 Author-email: tommymerlin0920@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,15 @@
 # 应用Secret
 CORPSECRET = ''
 # 应用ID
 AgentId = ''
 
 wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
 wn.send_msg("test message")
+wn.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
 wn.send_text_card("test title", "test content", "https://www.example.com")
 wn.send_file("./test.txt")
 wn.send_img("./test.png")
 
 # Webhook
 WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx"
 wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
@@ -74,16 +75,15 @@
 feishu.send_file(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "test.txt")
 
 # Webhook
 feishu_webhook = Nfeishu.FeishuWebhookNotify("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx")
 feishu_webhook.send_msg("Hello World!")
 ```
 
-### 飞书
-[官网](https://open.feishu.cn/document/server-docs/im-v1/introduction)  
+### 钉钉 
 [Webhook请求发送消息](https://open.dingtalk.com/document/robots/custom-robot-access)
 ```python
 from ANotify import Ndingtalk
 
 WEB_HOOK = "https://oapi.dingtalk.com/robot/send?access_token=xxxxxx"
 dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify(WEB_HOOK)
 dingtalk_webhook.send_msg("Hello World!")
```

#### html2text {}

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.1.0 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.1.1 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
 å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/)
 [ç¾¤èæºå¨äººWebhook](https://open.work.weixin.qq.com/help2/pc/14931)
 ```python from ANotify import Nwecom # ä¼ä¸ID CORPID = '' # åºç¨Secret
 CORPSECRET = '' # åºç¨ID AgentId = '' wn = Nwecom.WxNotify(corpid=CORPID,
 corpsecret=CORPSECRET, agentid=AgentId) wn.send_msg("test message")
-wn.send_text_card("test title", "test content", "https://www.example.com")
-wn.send_file("./test.txt") wn.send_img("./test.png") # Webhook WEB_HOOK =
-"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key=xxxxxx" wn_webhook =
-Nwecom.WxWebhookNotify(WEB_HOOK) wn_webhook.send_msg("Hello")
-wn_webhook.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://
-github.com/TommyMerlin/ANotify)") wn_webhook.send_img("E:/Desktop/gpt/
-Cursor_Demo/test.png") wn_webhook.send_file("test.png") ``` ### é£ä¹¦ [å®ç½]
-(https://open.feishu.cn/document/server-docs/im-v1/introduction) [åå»ºåºç¨]
-(https://open.feishu.cn/document/home/introduction-to-custom-app-development/
-self-built-application-development-process) [APIè°è¯å°](https://
-open.feishu.cn/api-explorer?from=op_doc_tab) [è·åæ¶æ¯åéå¯¹è±¡ openid]
-(https://open.feishu.cn/document/faq/trouble-shooting/how-to-obtain-openid)
-[Webhookè¯·æ±åéæ¶æ¯](https://open.feishu.cn/document/client-docs/bot-v3/
-add-custom-bot#355ec8c0) ```python from ANotify import Nfeishu APPID = ''
-APPSECRET = '' OPEN_ID = '' UNION_ID = '' USER_ID = '' CHAT_ID = '' feishu =
-Nfeishu.FeishuNotify(appid=APPID, appsecret=APPSECRET) feishu.send_msg
-(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "Hello World!") feishu.send_msg
-(Nfeishu.ReceiverType.UINION_ID, UNION_ID, "Hello World!") feishu.send_msg
-(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello World!") feishu.send_msg
-(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!") # åéå¾ç
-feishu.send_img(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID, "test.png") #
-åéæä»¶ feishu.send_file(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
-"test.txt") # Webhook feishu_webhook = Nfeishu.FeishuWebhookNotify("https://
-open.feishu.cn/open-apis/bot/v2/hook/xxxxxx") feishu_webhook.send_msg("Hello
-World!") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-docs/
-im-v1/introduction) [Webhookè¯·æ±åéæ¶æ¯](https://open.dingtalk.com/
-document/robots/custom-robot-access) ```python from ANotify import Ndingtalk
-WEB_HOOK = "https://oapi.dingtalk.com/robot/send?access_token=xxxxxx"
-dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify(WEB_HOOK)
-dingtalk_webhook.send_msg("Hello World!") ``` ### AnPush [å®ç½](https://
-anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
+wn.send_msg_markdown("**Hello**\n- test1\n- [ANotify](https://github.com/
+TommyMerlin/ANotify)") wn.send_text_card("test title", "test content", "https:/
+/www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png") #
+Webhook WEB_HOOK = "https://qyapi.weixin.qq.com/cgi-bin/webhook/
+send?key=xxxxxx" wn_webhook = Nwecom.WxWebhookNotify(WEB_HOOK)
+wn_webhook.send_msg("Hello") wn_webhook.send_msg_markdown("**Hello**\n-
+test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)")
+wn_webhook.send_img("E:/Desktop/gpt/Cursor_Demo/test.png") wn_webhook.send_file
+("test.png") ``` ### é£ä¹¦ [å®ç½](https://open.feishu.cn/document/server-
+docs/im-v1/introduction) [åå»ºåºç¨](https://open.feishu.cn/document/home/
+introduction-to-custom-app-development/self-built-application-development-
+process) [APIè°è¯å°](https://open.feishu.cn/api-explorer?from=op_doc_tab)
+[è·åæ¶æ¯åéå¯¹è±¡ openid](https://open.feishu.cn/document/faq/trouble-
+shooting/how-to-obtain-openid) [Webhookè¯·æ±åéæ¶æ¯](https://
+open.feishu.cn/document/client-docs/bot-v3/add-custom-bot#355ec8c0) ```python
+from ANotify import Nfeishu APPID = '' APPSECRET = '' OPEN_ID = '' UNION_ID =
+'' USER_ID = '' CHAT_ID = '' feishu = Nfeishu.FeishuNotify(appid=APPID,
+appsecret=APPSECRET) feishu.send_msg(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
+"Hello World!") feishu.send_msg(Nfeishu.ReceiverType.UINION_ID, UNION_ID,
+"Hello World!") feishu.send_msg(Nfeishu.ReceiverType.USER_ID, USER_ID, "Hello
+World!") feishu.send_msg(Nfeishu.ReceiverType.CHAT_ID, CHAT_ID, "Hello World!")
+# åéå¾ç feishu.send_img(Nfeishu.ReceiverType.OPEN_ID, OPEN_ID,
+"test.png") # åéæä»¶ feishu.send_file(Nfeishu.ReceiverType.OPEN_ID,
+OPEN_ID, "test.txt") # Webhook feishu_webhook = Nfeishu.FeishuWebhookNotify
+("https://open.feishu.cn/open-apis/bot/v2/hook/xxxxxx") feishu_webhook.send_msg
+("Hello World!") ``` ### éé [Webhookè¯·æ±åéæ¶æ¯](https://
+open.dingtalk.com/document/robots/custom-robot-access) ```python from ANotify
+import Ndingtalk WEB_HOOK = "https://oapi.dingtalk.com/robot/
+send?access_token=xxxxxx" dingtalk_webhook = Ndingtalk.DingtalkWebhookNotify
+(WEB_HOOK) dingtalk_webhook.send_msg("Hello World!") ``` ### AnPush [å®ç½]
+(https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
 Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
 ``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
 TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ```
 ### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from ANotify import
 NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus =
 Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
 "æµè¯æ­£æ", Npushplus.TemplateType.txt) msg_json = { "status": 200, "msg":
```

### Comparing `anotify-0.1.0/setup.py` & `anotify-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='anotify',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests>=2.15.1',
     ],
     author='7ommy',
     author_email='tommymerlin0920@gmail.com',
     description='Send notifications by multiple channels.',
```

