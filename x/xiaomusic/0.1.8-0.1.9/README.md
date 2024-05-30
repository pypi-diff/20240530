# Comparing `tmp/xiaomusic-0.1.8.tar.gz` & `tmp/xiaomusic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaomusic-0.1.8.tar", last modified: Sun Jan 28 11:04:17 2024, max compression
+gzip compressed data, was "xiaomusic-0.1.9.tar", last modified: Sun Jan 28 11:16:28 2024, max compression
```

## Comparing `xiaomusic-0.1.8.tar` & `xiaomusic-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/LICENSE
--rw-r--r--   0        0        0     1850 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/README.md
--rw-r--r--   0        0        0      524 2024-01-28 11:04:17.537561 xiaomusic-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/__init__.py
--rw-r--r--   0        0        0     1442 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/cli.py
--rw-r--r--   0        0        0     3400 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/config.py
--rw-r--r--   0        0        0     1488 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/httpserver.py
--rw-r--r--   0        0        0     1580 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/static/app.js
--rw-r--r--   0        0        0      660 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/static/index.html
--rw-r--r--   0        0        0    87533 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/static/jquery-3.7.1.min.js
--rw-r--r--   0        0        0     1822 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/utils.py
--rw-r--r--   0        0        0    17152 2024-01-28 11:04:10.537541 xiaomusic-0.1.8/xiaomusic/xiaomusic.py
--rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 xiaomusic-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1850 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/README.md
+-rw-r--r--   0        0        0      524 2024-01-28 11:16:28.735561 xiaomusic-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/__init__.py
+-rw-r--r--   0        0        0     1442 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/cli.py
+-rw-r--r--   0        0        0     3400 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/config.py
+-rw-r--r--   0        0        0     1488 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/httpserver.py
+-rw-r--r--   0        0        0     1580 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/static/app.js
+-rw-r--r--   0        0        0      660 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/static/index.html
+-rw-r--r--   0        0        0    87533 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/static/jquery-3.7.1.min.js
+-rw-r--r--   0        0        0     1822 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/utils.py
+-rw-r--r--   0        0        0    17152 2024-01-28 11:16:11.207492 xiaomusic-0.1.9/xiaomusic/xiaomusic.py
+-rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 xiaomusic-0.1.9/PKG-INFO
```

### Comparing `xiaomusic-0.1.8/LICENSE` & `xiaomusic-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/README.md` & `xiaomusic-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/pyproject.toml` & `xiaomusic-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xiaomusic"
-version = "0.1.8"
+version = "0.1.9"
 description = "Play Music with xiaomi AI speaker"
 authors = [
     { name = "涵曦", email = "im.hanxi@gmail.com" },
 ]
 dependencies = [
     "rich>=13.6.0",
     "requests>=2.31.0",
```

### Comparing `xiaomusic-0.1.8/xiaomusic/cli.py` & `xiaomusic-0.1.9/xiaomusic/cli.py`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/config.py` & `xiaomusic-0.1.9/xiaomusic/config.py`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/httpserver.py` & `xiaomusic-0.1.9/xiaomusic/httpserver.py`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/static/app.js` & `xiaomusic-0.1.9/xiaomusic/static/app.js`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/static/index.html` & `xiaomusic-0.1.9/xiaomusic/static/index.html`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/static/jquery-3.7.1.min.js` & `xiaomusic-0.1.9/xiaomusic/static/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/utils.py` & `xiaomusic-0.1.9/xiaomusic/utils.py`

 * *Files identical despite different names*

### Comparing `xiaomusic-0.1.8/xiaomusic/xiaomusic.py` & `xiaomusic-0.1.9/xiaomusic/xiaomusic.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,15 +450,15 @@
         (name, _) = os.path.splitext(os.path.basename(self.cur_music))
         self.log.debug("play_next. name:%s, cur_music:%s", name, self.cur_music)
         if self.play_type == PLAY_TYPE_ALL or name == "":
             name = self.random_music()
         if name == "":
             await self.do_tts(f"本地没有歌曲")
             return
-        await self.play(name=name)
+        await self.play(arg1=name)
 
     # 单曲循环
     async def set_play_type_one(self, **kwargs):
         self.play_type = PLAY_TYPE_ONE
         await self.do_tts(f"已经设置为单曲循环")
 
     # 全部循环
```

### Comparing `xiaomusic-0.1.8/PKG-INFO` & `xiaomusic-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaomusic
-Version: 0.1.8
+Version: 0.1.9
 Summary: Play Music with xiaomi AI speaker
 Author-Email: 涵曦 <im.hanxi@gmail.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: rich>=13.6.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: aiohttp>=3.8.6
```

