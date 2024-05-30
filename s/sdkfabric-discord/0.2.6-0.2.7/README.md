# Comparing `tmp/sdkfabric_discord-0.2.6.tar.gz` & `tmp/sdkfabric_discord-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_discord-0.2.6.tar", last modified: Thu May 23 21:16:53 2024, max compression
+gzip compressed data, was "sdkfabric_discord-0.2.7.tar", last modified: Thu May 30 18:51:45 2024, max compression
```

## Comparing `sdkfabric_discord-0.2.6.tar` & `sdkfabric_discord-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:53.815977 sdkfabric_discord-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 21:16:53.815977 sdkfabric_discord-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 21:16:50.000000 sdkfabric_discord-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:16:53.815977 sdkfabric_discord-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:53.811977 sdkfabric_discord-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:53.811977 sdkfabric_discord-0.2.6/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/channel_message_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/channel_reaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/channel_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/message_allowed_mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/message_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/message_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 21:16:49.000000 sdkfabric_discord-0.2.6/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:16:53.815977 sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 21:16:53.000000 sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 21:16:53.000000 sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:16:53.000000 sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:16:53.000000 sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:16:53.000000 sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:51:45.269084 sdkfabric_discord-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-30 18:51:45.269084 sdkfabric_discord-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:51:45.269084 sdkfabric_discord-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:51:45.265084 sdkfabric_discord-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:51:45.269084 sdkfabric_discord-0.2.7/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/channel_message_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/channel_reaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/channel_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/error_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/message_allowed_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/message_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/message_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-30 18:51:41.000000 sdkfabric_discord-0.2.7/src/sdk/user_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:51:45.269084 sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-30 18:51:45.000000 sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 18:51:45.000000 sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:51:45.000000 sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 18:51:45.000000 sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 18:51:45.000000 sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/top_level.txt
```

### Comparing `sdkfabric_discord-0.2.6/LICENSE` & `sdkfabric_discord-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/PKG-INFO` & `sdkfabric_discord-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-discord
-Version: 0.2.6
+Version: 0.2.7
 Summary: Discord Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/discord-python
 Project-URL: Issues, https://github.com/sdk-fabric/discord-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_discord-0.2.6/README.md` & `sdkfabric_discord-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/pyproject.toml` & `sdkfabric_discord-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-discord"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Discord Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_discord-0.2.6/src/sdk/channel.py` & `sdkfabric_discord-0.2.7/src/sdk/channel.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/src/sdk/channel_message_tag.py` & `sdkfabric_discord-0.2.7/src/sdk/channel_message_tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
+from .error_exception import ErrorException
 from .message import Message
 
 class ChannelMessageTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
@@ -36,14 +37,20 @@
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return List[Message].model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def get(self, channel_id: str, message_id: str) -> Message:
         """
@@ -63,14 +70,20 @@
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return Message.model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def create(self, channel_id: str, payload: Message) -> Message:
         """
@@ -90,14 +103,20 @@
             headers["Content-Type"] = "application/json"
 
             response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return Message.model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def update(self, channel_id: str, message_id: str, payload: Message) -> Message:
         """
@@ -118,14 +137,20 @@
             headers["Content-Type"] = "application/json"
 
             response = self.http_client.patch(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return Message.model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def remove(self, channel_id: str, message_id: str):
         """
@@ -145,14 +170,20 @@
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def crosspost(self, channel_id: str, message_id: str) -> Message:
         """
@@ -172,13 +203,19 @@
             headers = {}
 
             response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return Message.model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_discord-0.2.6/src/sdk/channel_reaction_tag.py` & `sdkfabric_discord-0.2.7/src/sdk/channel_reaction_tag.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
+from .error_exception import ErrorException
 from .user import User
 
 class ChannelReactionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
@@ -34,14 +35,20 @@
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return List[User].model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def delete_all(self, channel_id: str, message_id: str):
         try:
@@ -58,13 +65,19 @@
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_discord-0.2.6/src/sdk/channel_tag.py` & `sdkfabric_discord-0.2.7/src/sdk/channel_tag.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .channel import Channel
 from .channel_message_tag import ChannelMessageTag
 from .channel_reaction_tag import ChannelReactionTag
+from .error_exception import ErrorException
 from .message import Message
 
 class ChannelTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     def message(self) -> ChannelMessageTag:
@@ -47,14 +48,20 @@
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return Channel.model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def get_pins(self, channel_id: str) -> List[Message]:
         """
@@ -73,13 +80,19 @@
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
                 return List[Message].model_validate_json(json_data=response.content)
 
+            if response.status_code == 400:
+                raise ErrorException(response.content)
+            if response.status_code == 404:
+                raise ErrorException(response.content)
+            if response.status_code == 500:
+                raise ErrorException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_discord-0.2.6/src/sdk/client.py` & `sdkfabric_discord-0.2.7/src/sdk/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,24 +5,31 @@
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .channel_tag import ChannelTag
+from .user_tag import UserTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     def channel(self) -> ChannelTag:
         return ChannelTag(
             self.http_client,
             self.parser
         )
 
+    def user(self) -> UserTag:
+        return UserTag(
+            self.http_client,
+            self.parser
+        )
+
 
 
     @staticmethod
     def build(token: str):
         return Client("https://discord.com/api/v10", sdkgen.HttpBearer(token))
```

### Comparing `sdkfabric_discord-0.2.6/src/sdk/message.py` & `sdkfabric_discord-0.2.7/src/sdk/message.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/src/sdk/message_allowed_mentions.py` & `sdkfabric_discord-0.2.7/src/sdk/message_allowed_mentions.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/src/sdk/message_embed.py` & `sdkfabric_discord-0.2.7/src/sdk/message_embed.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/src/sdk/message_reference.py` & `sdkfabric_discord-0.2.7/src/sdk/message_reference.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/src/sdk/user.py` & `sdkfabric_discord-0.2.7/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/PKG-INFO` & `sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-discord
-Version: 0.2.6
+Version: 0.2.7
 Summary: Discord Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/discord-python
 Project-URL: Issues, https://github.com/sdk-fabric/discord-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_discord-0.2.6/src/sdkfabric_discord.egg-info/SOURCES.txt` & `sdkfabric_discord-0.2.7/src/sdkfabric_discord.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 pyproject.toml
 setup.py
 src/sdk/channel.py
 src/sdk/channel_message_tag.py
 src/sdk/channel_reaction_tag.py
 src/sdk/channel_tag.py
 src/sdk/client.py
+src/sdk/error.py
+src/sdk/error_exception.py
 src/sdk/message.py
 src/sdk/message_allowed_mentions.py
 src/sdk/message_embed.py
 src/sdk/message_reference.py
 src/sdk/user.py
+src/sdk/user_tag.py
 src/sdkfabric_discord.egg-info/PKG-INFO
 src/sdkfabric_discord.egg-info/SOURCES.txt
 src/sdkfabric_discord.egg-info/dependency_links.txt
 src/sdkfabric_discord.egg-info/requires.txt
 src/sdkfabric_discord.egg-info/top_level.txt
```

