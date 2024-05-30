# Comparing `tmp/stickersbot-4.1.1.tar.gz` & `tmp/stickersbot-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stickersbot-4.1.1.tar", last modified: Sat Apr 27 18:23:57 2024, max compression
+gzip compressed data, was "stickersbot-4.1.2.tar", last modified: Thu May 30 15:28:38 2024, max compression
```

## Comparing `stickersbot-4.1.1.tar` & `stickersbot-4.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.695646 stickersbot-4.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.691646 stickersbot-4.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-27 18:23:44.000000 stickersbot-4.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.691646 stickersbot-4.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-27 18:23:44.000000 stickersbot-4.1.1/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 18:23:44.000000 stickersbot-4.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-27 18:23:44.000000 stickersbot-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-27 18:23:57.695646 stickersbot-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-27 18:23:44.000000 stickersbot-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-27 18:23:44.000000 stickersbot-4.1.1/avatar.png
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-27 18:23:44.000000 stickersbot-4.1.1/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-27 18:23:44.000000 stickersbot-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:23:57.695646 stickersbot-4.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.691646 stickersbot-4.1.1/stickersbot/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-27 18:23:44.000000 stickersbot-4.1.1/stickersbot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:23:57.695646 stickersbot-4.1.1/stickersbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 18:23:57.000000 stickersbot-4.1.1/stickersbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:38.231802 stickersbot-4.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:38.227802 stickersbot-4.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 15:28:27.000000 stickersbot-4.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:38.227802 stickersbot-4.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-30 15:28:27.000000 stickersbot-4.1.2/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 15:28:27.000000 stickersbot-4.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-30 15:28:27.000000 stickersbot-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-30 15:28:38.231802 stickersbot-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 15:28:27.000000 stickersbot-4.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-30 15:28:27.000000 stickersbot-4.1.2/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 15:28:27.000000 stickersbot-4.1.2/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 15:28:27.000000 stickersbot-4.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:28:38.231802 stickersbot-4.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:38.227802 stickersbot-4.1.2/stickersbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 15:28:27.000000 stickersbot-4.1.2/stickersbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 15:28:27.000000 stickersbot-4.1.2/stickersbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-30 15:28:27.000000 stickersbot-4.1.2/stickersbot/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-30 15:28:27.000000 stickersbot-4.1.2/stickersbot/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-30 15:28:27.000000 stickersbot-4.1.2/stickersbot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:28:38.227802 stickersbot-4.1.2/stickersbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 15:28:38.000000 stickersbot-4.1.2/stickersbot.egg-info/top_level.txt
```

### Comparing `stickersbot-4.1.1/.github/workflows/python-ci.yml` & `stickersbot-4.1.2/.github/workflows/python-ci.yml`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/LICENSE` & `stickersbot-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/PKG-INFO` & `stickersbot-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stickersbot
-Version: 4.1.1
+Version: 4.1.2
 Summary: Sticker packs for all your Delta Chat needs
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/stickersbot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `stickersbot-4.1.1/README.md` & `stickersbot-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/avatar.png` & `stickersbot-4.1.2/avatar.png`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/pyproject.toml` & `stickersbot-4.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/stickersbot/hooks.py` & `stickersbot-4.1.2/stickersbot/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,28 +136,28 @@
 
 @cli.after(events.NewMessage)
 def delete_msgs(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     bot.rpc.delete_messages(accid, [event.msg.id])
 
 
 def process_signal_pack(bot: Bot, accid: int, msg: Message) -> None:
-    title, path = signal.download_pack(bot.account.get_blobdir(), msg.text)
-    size = os.stat(path).st_size
-    if size > 1024**2 * 15:
-        url = upload(bot.logger, path)
-        if url:
-            text = f"Name: {title}\nSize: {sizeof_fmt(size)}\nDownload: {url}"
+    with TemporaryDirectory() as tmp_dir:
+        title, path = signal.download_pack(tmp_dir, msg.text)
+        size = os.stat(path).st_size
+        if size > 1024**2 * 15:
+            url = upload(bot.logger, path)
+            if url:
+                text = f"Name: {title}\nSize: {sizeof_fmt(size)}\nDownload: {url}"
+            else:
+                text = f"❌ Pack too big ({sizeof_fmt(size)})"
+            reply = MsgData(text=text, quoted_message_id=msg.id)
+            bot.rpc.send_msg(accid, msg.chat_id, reply)
         else:
-            text = f"❌ Pack too big ({sizeof_fmt(size)})"
-        reply = MsgData(text=text, quoted_message_id=msg.id)
-        bot.rpc.send_msg(accid, msg.chat_id, reply)
-    else:
-        reply = MsgData(file=path, quoted_message_id=msg.id)
-        bot.rpc.send_msg(accid, msg.chat_id, reply)
-    os.remove(path)
+            reply = MsgData(file=path, quoted_message_id=msg.id)
+            bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
 def send_help(bot: Bot, accid: int, chatid: int) -> None:
     lines = [
         "Send me an image and I will remove the background and convert it to a Delta Chat sticker"
         " for you.\n",
         "Send me an emoji to get an sticker representing that emoji.\n",
```

### Comparing `stickersbot-4.1.1/stickersbot/signal.py` & `stickersbot-4.1.2/stickersbot/signal.py`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/stickersbot/util.py` & `stickersbot-4.1.2/stickersbot/util.py`

 * *Files identical despite different names*

### Comparing `stickersbot-4.1.1/stickersbot.egg-info/PKG-INFO` & `stickersbot-4.1.2/stickersbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stickersbot
-Version: 4.1.1
+Version: 4.1.2
 Summary: Sticker packs for all your Delta Chat needs
 Author-email: adbenitez <adb@merlinux.eu>
 Project-URL: Homepage, https://github.com/deltachat-bot/stickersbot
 Keywords: deltachat,bot
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

