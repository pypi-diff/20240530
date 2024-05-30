# Comparing `tmp/VodBot-1.1.8.tar.gz` & `tmp/VodBot-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VodBot-1.1.8.tar", last modified: Mon Aug  7 02:59:43 2023, max compression
+gzip compressed data, was "VodBot-1.1.9.tar", last modified: Mon Aug  7 21:26:11 2023, max compression
```

## Comparing `VodBot-1.1.8.tar` & `VodBot-1.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.480494 VodBot-1.1.8/
--rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.8/LICENSE.md
--rw-rw-rw-   0        0        0     4208 2023-08-07 02:59:43.479488 VodBot-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.454381 VodBot-1.1.8/VodBot.egg-info/
--rw-rw-rw-   0        0        0     4208 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      198 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-07 02:59:43.000000 VodBot-1.1.8/VodBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 02:59:43.480494 VodBot-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.465559 VodBot-1.1.8/vodbot/
--rw-rw-rw-   0        0        0       47 2023-08-07 02:59:06.000000 VodBot-1.1.8/vodbot/__init__.py
--rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.8/vodbot/__main__.py
--rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.8/vodbot/cache.py
--rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.8/vodbot/chatlog.py
-drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.474294 VodBot-1.1.8/vodbot/commands/
--rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.8/vodbot/commands/__init__.py
--rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.8/vodbot/commands/export.py
--rw-rw-rw-   0        0        0     3460 2023-05-03 01:36:40.000000 VodBot-1.1.8/vodbot/commands/info.py
--rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.8/vodbot/commands/init.py
--rw-rw-rw-   0        0        0     7901 2023-04-17 22:07:30.000000 VodBot-1.1.8/vodbot/commands/pull.py
--rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.8/vodbot/commands/stage.py
--rw-rw-rw-   0        0        0    12978 2023-05-03 01:01:36.000000 VodBot-1.1.8/vodbot/commands/upload.py
--rw-rw-rw-   0        0        0    16532 2023-05-06 00:49:37.000000 VodBot-1.1.8/vodbot/config.py
-drwxrwxrwx   0        0        0        0 2023-08-07 02:59:43.478981 VodBot-1.1.8/vodbot/itd/
--rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.8/vodbot/itd/__init__.py
--rw-rw-rw-   0        0        0     3372 2023-05-03 01:01:36.000000 VodBot-1.1.8/vodbot/itd/download.py
--rw-rw-rw-   0        0        0     4231 2023-08-07 02:29:41.000000 VodBot-1.1.8/vodbot/itd/gql.py
--rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.8/vodbot/itd/worker.py
--rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.8/vodbot/printer.py
--rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.8/vodbot/thumbnail.py
--rw-rw-rw-   0        0        0    10291 2023-08-07 02:29:32.000000 VodBot-1.1.8/vodbot/twitch.py
--rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.8/vodbot/util.py
--rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.8/vodbot/video.py
--rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.8/vodbot/webhook.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:26:11.173307 VodBot-1.1.9/
+-rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.9/LICENSE.md
+-rw-rw-rw-   0        0        0     4208 2023-08-07 21:26:11.172298 VodBot-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 21:26:11.145351 VodBot-1.1.9/VodBot.egg-info/
+-rw-rw-rw-   0        0        0     4208 2023-08-07 21:26:11.000000 VodBot-1.1.9/VodBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-07 21:26:11.000000 VodBot-1.1.9/VodBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 21:26:11.000000 VodBot-1.1.9/VodBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-08-07 21:26:11.000000 VodBot-1.1.9/VodBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      198 2023-08-07 21:26:11.000000 VodBot-1.1.9/VodBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 21:26:11.000000 VodBot-1.1.9/VodBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 21:26:11.173814 VodBot-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:26:11.159538 VodBot-1.1.9/vodbot/
+-rw-rw-rw-   0        0        0       47 2023-08-07 20:35:00.000000 VodBot-1.1.9/vodbot/__init__.py
+-rw-rw-rw-   0        0        0     9263 2023-08-07 20:01:32.000000 VodBot-1.1.9/vodbot/__main__.py
+-rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.9/vodbot/cache.py
+-rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.9/vodbot/chatlog.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:26:11.167612 VodBot-1.1.9/vodbot/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.9/vodbot/commands/__init__.py
+-rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.9/vodbot/commands/export.py
+-rw-rw-rw-   0        0        0     3460 2023-05-03 01:36:40.000000 VodBot-1.1.9/vodbot/commands/info.py
+-rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.9/vodbot/commands/init.py
+-rw-rw-rw-   0        0        0     8303 2023-08-07 20:28:30.000000 VodBot-1.1.9/vodbot/commands/pull.py
+-rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.9/vodbot/commands/stage.py
+-rw-rw-rw-   0        0        0    13003 2023-08-07 16:37:33.000000 VodBot-1.1.9/vodbot/commands/upload.py
+-rw-rw-rw-   0        0        0    16735 2023-08-07 19:04:08.000000 VodBot-1.1.9/vodbot/config.py
+drwxrwxrwx   0        0        0        0 2023-08-07 21:26:11.171189 VodBot-1.1.9/vodbot/itd/
+-rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.9/vodbot/itd/__init__.py
+-rw-rw-rw-   0        0        0     3372 2023-05-03 01:01:36.000000 VodBot-1.1.9/vodbot/itd/download.py
+-rw-rw-rw-   0        0        0     4289 2023-08-07 19:59:19.000000 VodBot-1.1.9/vodbot/itd/gql.py
+-rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.9/vodbot/itd/worker.py
+-rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.9/vodbot/printer.py
+-rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.9/vodbot/thumbnail.py
+-rw-rw-rw-   0        0        0    10868 2023-08-07 20:03:30.000000 VodBot-1.1.9/vodbot/twitch.py
+-rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.9/vodbot/util.py
+-rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.9/vodbot/video.py
+-rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.9/vodbot/webhook.py
```

### Comparing `VodBot-1.1.8/LICENSE.md` & `VodBot-1.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/PKG-INFO` & `VodBot-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.8
+Version: 1.1.9
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
```

### Comparing `VodBot-1.1.8/README.md` & `VodBot-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/VodBot.egg-info/PKG-INFO` & `VodBot-1.1.9/VodBot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.8
+Version: 1.1.9
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
```

### Comparing `VodBot-1.1.8/VodBot.egg-info/SOURCES.txt` & `VodBot-1.1.9/VodBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/setup.py` & `VodBot-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/__main__.py` & `VodBot-1.1.9/vodbot/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from . import util, __project__, __version__
 from .config import DEFAULT_CONFIG_PATH
 from .printer import colorize
 from .cache import load_cache
+from .itd import gql
 
 import argparse
 import argcomplete
 from argcomplete.completers import FilesCompleter, DirectoriesCompleter
 from pathlib import Path
 from importlib import import_module
 from requests.exceptions import ConnectionError
@@ -173,15 +174,20 @@
 	if ffmpeg_check is None:
 		util.exit_prog(-11, "FFmpeg could not be found in your PATH environment variable.")
 
 	# Handle commands
 	if args.cmd == "init":
 		import_module(".commands.init", "vodbot").run(args)
 	elif args.cmd == "pull" or args.cmd == "download":
-		import_module(".commands.pull", "vodbot").run(args)
+		try:
+			import_module(".commands.pull", "vodbot").run(args)
+		except gql.GQLItemError as e:
+			util.exit_prog(53, f"Failed to query a specific item using GQL: {e}")
+		except gql.GQLException as e:
+			util.exit_prog(54, f"Generic GQL Exception: {e}")
 	elif args.cmd == "stage":
 		import_module(".commands.stage", "vodbot").run(args)
 	elif args.cmd == "push" or args.cmd == "upload":
 		import_module(".commands.upload", "vodbot").run(args)
 	elif args.cmd == "export" or args.cmd == "slice":
 		import_module(".commands.export", "vodbot").run(args)
 	elif args.cmd == "info":
```

### Comparing `VodBot-1.1.8/vodbot/cache.py` & `VodBot-1.1.9/vodbot/cache.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/chatlog.py` & `VodBot-1.1.9/vodbot/chatlog.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/commands/export.py` & `VodBot-1.1.9/vodbot/commands/export.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/commands/info.py` & `VodBot-1.1.9/vodbot/commands/info.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/commands/init.py` & `VodBot-1.1.9/vodbot/commands/init.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/commands/pull.py` & `VodBot-1.1.9/vodbot/commands/pull.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,29 +4,36 @@
 from vodbot import util, twitch
 from vodbot.itd import download as itd_dl, worker as itd_work
 from vodbot.printer import cprint
 from vodbot.itd.gql import set_client_id
 from vodbot.cache import Cache, load_cache, save_cache, _CacheChannel
 from vodbot.webhook import init_webhooks, send_pull_clip, send_pull_error, send_pull_job_done, send_pull_vod
 
-from pathlib import Path
 from os import listdir
 from os.path import isfile
 
 
 def run(args):
 	# Load the config and set up the access token
 	cprint("#r#dLoading config...#r", end=" ", flush=True)
 	conf = util.load_conf(args.config)
+	if conf.pull.gql_client == "kimne78kx3ncx6brgo4mv6wki5h1ko":
+		cprint("""#r#fY
+WARNING: You appear to be using the old Twitch GQL Client ID,
+"kimne78kx3ncx6brgo4mv6wki5h1ko". This specific client ID has been recently
+known to cause issues and be generally unreliable. It is highly reocmmended you
+switch to a different one such as "kd1unb4b3q4t58fwlpcbzcbnm76a8fp". This can
+be changed in your configuration file, read more on the wiki page on GitHub.
+#r""")
+
 	cache: Cache = load_cache(conf, args.cache_toggle)
 	init_webhooks(conf)
 	VODS_DIR = conf.directories.vods
 	CLIPS_DIR = conf.directories.clips
 	TEMP_DIR = conf.directories.temp
-	LOG_LEVEL = conf.export.ffmpeg_loglevel
 	PULL_CHAT = conf.pull.save_chat
 	set_client_id(conf.pull.gql_client)
 	
 	cprint("#r#dLoading channel data...#r", end=" ", flush=True)
 	# This function is actually useless, we don't need anything from it, just the channel login name which we already have.
 	# TODO: remove this useless query entirely, nothing from it is used that we don't already have.
 	channels: List[twitch.Channel] = [] #twitch.get_channels([channel.username for channel in conf.channels])
```

### Comparing `VodBot-1.1.8/vodbot/commands/stage.py` & `VodBot-1.1.9/vodbot/commands/stage.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/commands/upload.py` & `VodBot-1.1.9/vodbot/commands/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,17 @@
 	video_id = "" # youtube video id
 	resp = None
 	errn = 0
 	errn_max = 10
 
 	uploaded = 0
 
-	def print_error(f:List, secs:int = 5):
+	def print_error(f:List, secs:int=5):
 		nonlocal errn, errn_max
+		f = [str(x) for x in f]
 		cprint(f"#fY#dWARN: An HTTP error has occurred ({errn}/{errn_max}), retyring in {secs} seconds... ({', '.join(f)})#r")
 		errn += 1
 		sleep(secs)
 
 	while resp is None:
 		try:
 			status, resp = response_upload.next_chunk()
```

### Comparing `VodBot-1.1.8/vodbot/config.py` & `VodBot-1.1.9/vodbot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,18 @@
 	# Determines if chat logs get pulled with VODs and saved alongside metadata. This is a master
 	# switch for every channel, if false then no chat gets saved.
 	save_chat: bool = True
 
 	# Client ID for accessing Twitch's public facing but privately documented GraphQL interface, 
 	# which is significantly more advanced than the V5 API. Do not change this to a specific user's
 	# ID unless you want to risk a ban, although it allows for accessing private info such as
-	# deleted chat messages and account info. Recommended values (public client ID's) are
-	# "kimne78kx3ncx6brgo4mv6wki5h1ko" or "kd1unb4b3q4t58fwlpcbzcbnm76a8fp".
+	# deleted chat messages and account info. Recommended value (public client ID's) is
+	# "kd1unb4b3q4t58fwlpcbzcbnm76a8fp". Only use "kimne78kx3ncx6brgo4mv6wki5h1ko" if you absolutely
+	# know what you're doing! It appears to be more locked down than the new client ID. I've wasted
+	# many, many hours on issues rooted with this client ID. You have been warned!!!
 	gql_client: str = "kd1unb4b3q4t58fwlpcbzcbnm76a8fp"
 
 	# Number of threads that can concurrently work to download files from Twitch.
 	# Defaults to the number of cores on the machine (or 1 in cases where that can't be measured).
 	max_workers: int = field(default=cpu_count() or 1, metadata=config(mm_field=fields.Int(validate=validate.Range(1))))
 	# Number of bytes to stream-write to temporary video files at a time.
 	# Defaults to 1024 bytes.
```

### Comparing `VodBot-1.1.8/vodbot/itd/download.py` & `VodBot-1.1.9/vodbot/itd/download.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/itd/gql.py` & `VodBot-1.1.9/vodbot/itd/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 GQL_HEADERS = {"Client-ID": ""}
 
 
 class GQLException(Exception):
 	pass
 
 
+class GQLItemError(Exception):
+	pass
+
+
 # We use Twitch's private client ID for GQL calls
 def set_client_id(client_id: str):
 	global GQL_HEADERS
 	GQL_HEADERS["Client-ID"] = client_id
 
 
 def _process_query_errors(resp):
@@ -35,38 +39,39 @@
 	return gql_post(json={"query":query}, data=data)
 
 
 # GQL Query forms
 # Channel VODs query
 GET_CHANNEL_VIDEOS_QUERY = """
 {{  user(login: "{channel_id}") {{
-		videos( first: {first}, sort: {sort}, after: "{after}" ) {{
+		videos( first: {first}, sort: {sort}, after: {after} ) {{
 			totalCount
 			edges {{ cursor
 				node {{
 					id title publishedAt broadcastType status lengthSeconds
 					game {{ id name }}
 					creator {{ id login displayName }}
 }}  }}  }}  }}  }}
 """
 # Channel Clips query
 # period can be LAST_DAY, LAST_WEEK, LAST_MONTH, or ALL_TIME
 GET_CHANNEL_CLIPS_QUERY = """
 {{  user(login: "{channel_id}") {{
 		clips(
-			first: {first}, after: "{after}",
-			criteria: {{ period: ALL_TIME, sort: CREATED_AT_DESC }}
+			first: {first}, after: {after},
+			criteria: {{ period: ALL_TIME, sort: VIEWS_DESC }}
 		) {{
-			edges {{ cursor
-				node {{ id slug title createdAt viewCount
-					durationSeconds videoOffsetSeconds
-					video {{ id }}
-					game {{ id name }}
-					broadcaster {{ id displayName login }}
-					curator {{ id displayName login }}
+			pageInfo {{ hasNextPage }}
+			edges {{ cursor node {{
+				id slug title createdAt viewCount
+				durationSeconds videoOffsetSeconds
+				video {{ id }}
+				game {{ id name }}
+				broadcaster {{ id displayName login }}
+				curator {{ id displayName login }}
 }}  }}  }}  }}  }}
 """
 # Single VOD query
 GET_VIDEO_QUERY = """
 {{  video(id: "{video_id}") {{
 		id title publishedAt
 		broadcastType lengthSeconds
@@ -92,15 +97,15 @@
 		stream {{
 			id title type viewersCount createdAt game {{ id name }}
 }}  }}  }}
 """
 # IRC Chat query
 GET_VIDEO_COMMENTS_QUERY = """
 {{ video(id: "{video_id}") {{
-	comments(contentOffsetSeconds: 0, after: "{after}") {{
+	comments(contentOffsetSeconds: 0, after: {after}) {{
 		edges {{ cursor node {{
 			contentOffsetSeconds
 			commenter {{ displayName }}
 			message {{ userColor fragments {{ mention {{ displayName }} text }} }}
 }}  }}  }}  }} }}
 """
 # VOD chapters query
```

### Comparing `VodBot-1.1.8/vodbot/itd/worker.py` & `VodBot-1.1.9/vodbot/itd/worker.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/printer.py` & `VodBot-1.1.9/vodbot/printer.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/thumbnail.py` & `VodBot-1.1.9/vodbot/thumbnail.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/twitch.py` & `VodBot-1.1.9/vodbot/twitch.py`

 * *Files 11% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 	channels = []
 	for channel_login in channel_logins:
 		query = gql.GET_CHANNEL_QUERY.format(channel_login=channel_login)
 		resp = gql.gql_query(query=query).json()
 		c = resp["data"]["user"]
 
 		if c == None:
-			raise Exception(f"Channel `{channel_login}` does not exist!")
+			raise gql.GQLItemError(f"Channel `{channel_login}` does not exist!")
 		
 		channels.append(
 			Channel(
 				id=c["id"], login=c["login"],
 				display_name=c["displayName"], created_at=c["createdAt"]
 			)
 		)
@@ -192,30 +192,35 @@
 	Uses a (blocking) HTTP request to retrieve VOD info for a specific channel.
 
 	:param channel: A Channel object.
 	:returns: A list of VOD objects.
 	"""
 
 	vods = []
-	pagination = ""
+	pagination = "null"
+
 	while True:
 		# get videos of multiple types
 		# past streams = ARCHIVE, segment of stream = HIGHLIGHT, upload = UPLOAD, premiere = PAST_PREMIERE
 		query = gql.GET_CHANNEL_VIDEOS_QUERY.format(
 			channel_id=channel.login,
 			after=pagination, first=100,
 			sort="TIME"
 		)
 		resp = gql.gql_query(query=query).json()
+
+		if not resp["data"]["user"]:
+			raise gql.GQLItemError(f"Failed to find channel videos for `{channel.login}`.")
+
 		resp = resp["data"]["user"]["videos"]
 
 		if not resp or not resp["edges"]:
 			break
 
-		pagination = resp["edges"][-1]["cursor"]
+		tempcursor = resp["edges"][-1]["cursor"]
 		
 		for vod in resp["edges"]:
 			v = vod["node"]
 			c, g, b, s = v["creator"], v["game"], v["broadcastType"], v["status"]
 
 			# check broadcast type
 			if not any(b==t for t in ["ARCHIVE", "HIGHLIGHT", "UPLOAD", "PAST_PREMIERE"]):
@@ -230,78 +235,91 @@
 			if g:
 				game_id, game_name = g["id"], g["name"]
 			
 			
 			# Get stream chapter info now
 			chapters = []
 			chapter_page = "null"
+
 			while True:
 				query = gql.GET_VIDEO_CHAPTERS.format(
 					id=v["id"], after=chapter_page
 				)
 				resp = gql.gql_query(query=query).json()
+				
+				if not resp["data"]["video"]:
+					raise gql.GQLItemError(f"Failed to find moments for video `{v['id']}`.")
+				
 				resp = resp["data"]["video"]["moments"]
 				
-				if not resp or not resp["edges"] or not resp["edges"][-1]["cursor"]:
+				if not resp or not resp["edges"]:
 					break
 
-				chapter_page = f'"{resp["edges"][-1]["cursor"]}"'
-
 				for chap in resp["edges"]:
 					n = chap["node"]
 					chapters.append(
 						VodChapter(
 							type=n["type"], description=n["description"],
 							position=int(n["positionMilliseconds"]/1000),
 							duration=int(n["durationMilliseconds"]/1000)
 							# its fine to do the above because twitch's precision of message timings isnt greater than seconds
 						)
 					)
 				
 				if chapter_page == "" or chapter_page == None:
 					break
+				
+				if not resp["edges"][-1]["cursor"]:
+					break
+
+				chapter_page = '"' + resp["edges"][-1]["cursor"] + '"'
 
 			vods.append(
 				Vod(
 					id=v["id"], length=v["lengthSeconds"], title=v["title"],
 					user_id=c["id"], user_login=c["login"], user_name=c["displayName"], 
 					game_id=game_id, game_name=game_name, created_at=v["publishedAt"],
 					chapters=chapters
 				)
 			)
 
-		if pagination == "" or pagination == None:
+		if not tempcursor:
 			break
 
+		pagination = '"' + tempcursor + '"'
+
 
 	return vods
 
 
 def get_channel_clips(channel: Channel) -> List[Clip]:
 	"""
 	Uses a (blocking) HTTP request to retrieve Clip info for a specific channel.
 
 	:param channel: A Channel object.
 	:returns: A list of Clip objects.
 	"""
 
 	clips = []
-	pagination = ""
+	pagination = "null"
 	
 	while True:
 		query = gql.GET_CHANNEL_CLIPS_QUERY.format(
 			channel_id=channel.login,
 			after=pagination, first=100
 		)
-		resp = gql.gql_query(query=query).json()["data"]["user"]["clips"]
+		resp = gql.gql_query(query=query).json()
+
+		if not resp["data"]["user"]:
+			raise gql.GQLItemError(f"Failed to find channel clips for `{channel.login}`.")
+		
+		resp = resp["data"]["user"]["clips"]
 
 		if not resp or not resp["edges"]:
 			break
-
-		pagination = {resp["edges"][-1]["cursor"]}
 		
 		for clip in resp["edges"]:
 			c = clip["node"]
 			b, w, g, v = c["broadcaster"], c["curator"], c["game"], c["video"]
 			v_id = "unknown" if v is None else v["id"]
 
 			w_id, w_login, w_name = b["id"], b["login"], b["displayName"]
@@ -322,43 +340,47 @@
 					clipper_id=w_id, clipper_login=w_login, clipper_name=w_name,
 					game_id=g_id, game_name=g_name, title=c["title"],
 					view_count=c["viewCount"], length=c["durationSeconds"],
 					offset=c["videoOffsetSeconds"] or 0, video_id=v_id
 				)
 			)
 
-		if pagination == "" or pagination == None:
+		if not resp["edges"][-1]["cursor"]:
 			break
 
+		pagination = '"' + resp["edges"][-1]["cursor"] + '"'
+
 	return clips
 
 
 def get_video_comments(video_id: str) -> List[ChatMessage]:
 	"""
 	Uses a (blocking) HTTP request to retrieve chat logs for a specific video.
 
 	:param video_id: A video ID string.
 	:returns: A list of ChatMessage objects.
 	"""
 
 	messages = []
-	pagination = ""
+	pagination = "null"
 
 	while True:
 		query = gql.GET_VIDEO_COMMENTS_QUERY.format(
 			video_id=video_id, first=100, after=pagination
 		)
 		resp = gql.gql_query(query=query).json()
+		
+		if not resp["data"]["video"]:
+			raise gql.GQLItemError(f"Failed to find comments for video `{video_id}`.")
+		
 		resp = resp["data"]["video"]["comments"]
 
 		if not resp or not resp["edges"]:
 			break
 
-		pagination = {resp["edges"][-1]["cursor"]}
-
 		for comment in resp["edges"]:
 			c = comment["node"]
 			
 			usr = "-BANNED?_USER-"
 			if c["commenter"] is not None:
 				usr = c["commenter"]["displayName"]
 			
@@ -375,11 +397,13 @@
 			messages.append(
 				ChatMessage(
 					user=usr, color=clr, msg=msg,
 					offset=c["contentOffsetSeconds"]
 				)
 			)
 		
-		if pagination == "" or pagination == None:
+		if not resp["edges"][-1]["cursor"]:
 			break
+
+		pagination = '"' + resp["edges"][-1]["cursor"] + '"'
 	
 	return messages
```

### Comparing `VodBot-1.1.8/vodbot/util.py` & `VodBot-1.1.9/vodbot/util.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/video.py` & `VodBot-1.1.9/vodbot/video.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.8/vodbot/webhook.py` & `VodBot-1.1.9/vodbot/webhook.py`

 * *Files identical despite different names*

