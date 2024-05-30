# Comparing `tmp/spotipy-2.8.0.tar.gz` & `tmp/spotipy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spotipy-2.8.0.tar", last modified: Wed Feb 12 22:41:21 2020, max compression
+gzip compressed data, was "dist/spotipy-2.9.0.tar", last modified: Sat Feb 15 19:47:23 2020, max compression
```

## Comparing `spotipy-2.8.0.tar` & `spotipy-2.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/
--rw-r--r--   0 stephane.bruckert (87869827) 939931750       43 2020-01-11 19:53:23.000000 spotipy-2.8.0/MANIFEST.in
--rw-r--r--   0 stephane.bruckert (87869827) 939931750     2101 2020-02-12 22:41:21.000000 spotipy-2.8.0/PKG-INFO
--rw-r--r--   0 stephane.bruckert (87869827) 939931750     1483 2020-02-12 22:31:22.000000 spotipy-2.8.0/README.md
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/docs/
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/docs/_build/
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/docs/_build/html/
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/docs/_build/html/_sources/
--rw-r--r--   0 stephane.bruckert (87869827) 939931750    12003 2020-01-12 14:22:41.000000 spotipy-2.8.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 stephane.bruckert (87869827) 939931750       40 2020-01-15 18:59:08.000000 spotipy-2.8.0/requirements.txt
--rw-r--r--   0 stephane.bruckert (87869827) 939931750       38 2020-02-12 22:41:21.000000 spotipy-2.8.0/setup.cfg
--rw-r--r--   0 stephane.bruckert (87869827) 939931750      545 2020-02-12 22:37:42.000000 spotipy-2.8.0/setup.py
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy/
--rw-r--r--   0 stephane.bruckert (87869827) 939931750       88 2020-01-12 13:24:40.000000 spotipy-2.8.0/spotipy/__init__.py
--rw-r--r--   0 stephane.bruckert (87869827) 939931750    46645 2020-02-12 22:17:50.000000 spotipy-2.8.0/spotipy/client.py
--rw-r--r--   0 stephane.bruckert (87869827) 939931750    13393 2020-02-12 22:26:38.000000 spotipy-2.8.0/spotipy/oauth2.py
--rw-r--r--   0 stephane.bruckert (87869827) 939931750     2898 2020-02-12 22:17:50.000000 spotipy-2.8.0/spotipy/util.py
-drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy.egg-info/
--rw-r--r--   0 stephane.bruckert (87869827) 939931750     2101 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy.egg-info/PKG-INFO
--rw-r--r--   0 stephane.bruckert (87869827) 939931750      313 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy.egg-info/SOURCES.txt
--rw-r--r--   0 stephane.bruckert (87869827) 939931750        1 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy.egg-info/dependency_links.txt
--rw-r--r--   0 stephane.bruckert (87869827) 939931750       29 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy.egg-info/requires.txt
--rw-r--r--   0 stephane.bruckert (87869827) 939931750        8 2020-02-12 22:41:21.000000 spotipy-2.8.0/spotipy.egg-info/top_level.txt
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750       43 2020-01-11 19:53:23.000000 spotipy-2.9.0/MANIFEST.in
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750     2099 2020-02-15 19:47:23.000000 spotipy-2.9.0/PKG-INFO
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750     1481 2020-02-15 19:47:04.000000 spotipy-2.9.0/README.md
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/docs/
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/docs/_build/
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/docs/_build/html/
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/docs/_build/html/_sources/
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750    12003 2020-01-12 14:22:41.000000 spotipy-2.9.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750       40 2020-01-15 18:59:08.000000 spotipy-2.9.0/requirements.txt
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750       38 2020-02-15 19:47:23.000000 spotipy-2.9.0/setup.cfg
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750      545 2020-02-15 19:47:13.000000 spotipy-2.9.0/setup.py
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy/
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750       88 2020-01-12 13:24:40.000000 spotipy-2.9.0/spotipy/__init__.py
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750    47080 2020-02-12 23:34:40.000000 spotipy-2.9.0/spotipy/client.py
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750    13897 2020-02-15 19:44:10.000000 spotipy-2.9.0/spotipy/oauth2.py
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750     2898 2020-02-12 22:17:50.000000 spotipy-2.9.0/spotipy/util.py
+drwxr-xr-x   0 stephane.bruckert (87869827) 939931750        0 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy.egg-info/
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750     2099 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy.egg-info/PKG-INFO
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750      313 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy.egg-info/SOURCES.txt
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750        1 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy.egg-info/dependency_links.txt
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750       29 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy.egg-info/requires.txt
+-rw-r--r--   0 stephane.bruckert (87869827) 939931750        8 2020-02-15 19:47:23.000000 spotipy-2.9.0/spotipy.egg-info/top_level.txt
```

### Comparing `spotipy-2.8.0/PKG-INFO` & `spotipy-2.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy
-Version: 2.8.0
+Version: 2.9.0
 Summary: A light weight Python library for the Spotify Web API
 Home-page: http://spotipy.readthedocs.org/
 Author: @plamere
 Author-email: paul@echonest.com
 License: LICENSE.md
 Description: # Spotipy
         
@@ -26,15 +26,15 @@
         
         To get started, install spotipy and create an app on https://developers.spotify.com/.
         Add your new ID and SECRET to your environment:
         
             export SPOTIPY_CLIENT_ID=client_id_here
             export SPOTIPY_CLIENT_SECRET=client_secret_here
         
-            // on Windows, use `SET` instead of `export`).
+            // on Windows, use `SET` instead of `export`
         
         Then, create a Spotify object and call methods:
         
             import spotipy
             from spotipy.oauth2 import SpotifyClientCredentials
         
             sp = spotipy.Spotify(client_credentials_manager=SpotifyClientCredentials())
```

### Comparing `spotipy-2.8.0/README.md` & `spotipy-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 To get started, install spotipy and create an app on https://developers.spotify.com/.
 Add your new ID and SECRET to your environment:
 
     export SPOTIPY_CLIENT_ID=client_id_here
     export SPOTIPY_CLIENT_SECRET=client_secret_here
 
-    // on Windows, use `SET` instead of `export`).
+    // on Windows, use `SET` instead of `export`
 
 Then, create a Spotify object and call methods:
 
     import spotipy
     from spotipy.oauth2 import SpotifyClientCredentials
 
     sp = spotipy.Spotify(client_credentials_manager=SpotifyClientCredentials())
```

### Comparing `spotipy-2.8.0/docs/_build/html/_sources/index.rst.txt` & `spotipy-2.9.0/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `spotipy-2.8.0/setup.py` & `spotipy-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='spotipy',
-    version='2.8.0',
+    version='2.9.0',
     description='A light weight Python library for the Spotify Web API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="@plamere",
     author_email="paul@echonest.com",
     url='http://spotipy.readthedocs.org/',
     install_requires=[
```

### Comparing `spotipy-2.8.0/spotipy/client.py` & `spotipy-2.9.0/spotipy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1166,15 +1166,15 @@
                 - force_play - true: after transfer, play. false:
                                keep current state.
         """
         data = {"device_ids": [device_id], "play": force_play}
         return self._put("me/player", payload=data)
 
     def start_playback(
-        self, device_id=None, context_uri=None, uris=None, offset=None
+        self, device_id=None, context_uri=None, uris=None, offset=None, position_ms=None
     ):
         """ Start or resume user's playback.
 
             Provide a `context_uri` to start playback or a album,
             artist, or playlist.
 
             Provide a `uris` list to start playback of one or more
@@ -1184,28 +1184,34 @@
             to start playback at a particular offset.
 
             Parameters:
                 - device_id - device target for playback
                 - context_uri - spotify context uri to play
                 - uris - spotify track uris
                 - offset - offset into context by index or track
+                - position_ms - (optional) indicates from what position to start playback.
+                                Must be a positive number. Passing in a position that is
+                                greater than the length of the track will cause the player to
+                                start playing the next song.
         """
         if context_uri is not None and uris is not None:
             self._warn("specify either context uri or uris, not both")
             return
         if uris is not None and not isinstance(uris, list):
             self._warn("uris must be a list")
             return
         data = {}
         if context_uri is not None:
             data["context_uri"] = context_uri
         if uris is not None:
             data["uris"] = uris
         if offset is not None:
             data["offset"] = offset
+        if position_ms is not None:
+            data["position_ms"] = position_ms
         return self._put(
             self._append_device_id("me/player/play", device_id), payload=data
         )
 
     def pause_playback(self, device_id=None):
         """ Pause user's playback.
```

### Comparing `spotipy-2.8.0/spotipy/oauth2.py` & `spotipy-2.9.0/spotipy/oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,25 +77,26 @@
     def redirect_uri(self, val):
         self._redirect_uri = _ensure_value(val, "redirect_uri")
 
 
 class SpotifyClientCredentials(SpotifyAuthBase):
     OAUTH_TOKEN_URL = "https://accounts.spotify.com/api/token"
 
-    def __init__(self, client_id=None, client_secret=None, proxies=None):
+    def __init__(self, client_id=None, client_secret=None, proxies=None, requests_timeout=None):
         """
         You can either provide a client_id and client_secret to the
         constructor or set SPOTIPY_CLIENT_ID and SPOTIPY_CLIENT_SECRET
         environment variables
         """
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.token_info = None
         self.proxies = proxies
+        self.requests_timeout = requests_timeout
 
     def get_access_token(self, as_dict=True):
         """
         If a valid access token is in memory, returns it
         Else feches a new token and returns it
 
             Parameters:
@@ -133,14 +134,15 @@
 
         response = requests.post(
             self.OAUTH_TOKEN_URL,
             data=payload,
             headers=headers,
             verify=True,
             proxies=self.proxies,
+            timeout=self.requests_timeout,
         )
         if response.status_code != 200:
             raise SpotifyOauthError(response.reason)
         token_info = response.json()
         return token_info
 
     def is_token_expired(self, token_info):
@@ -169,39 +171,43 @@
         client_secret=None,
         redirect_uri=None,
         state=None,
         scope=None,
         cache_path=None,
         username=None,
         proxies=None,
-        show_dialog=False
+        show_dialog=False,
+        requests_timeout=None
     ):
         """
             Creates a SpotifyOAuth object
 
             Parameters:
                  - client_id - the client id of your app
                  - client_secret - the client secret of your app
                  - redirect_uri - the redirect URI of your app
                  - state - security state
                  - scope - the desired scope of the request
                  - cache_path - path to location to save tokens
+                 - requests_timeout - tell Requests to stop waiting for a response
+                                      after a given number of seconds
                  - username - username of current client
         """
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.state = state
         self.cache_path = cache_path
         self.username = username or os.getenv(
             CLIENT_CREDS_ENV_VARS["client_username"]
         )
         self.scope = self._normalize_scope(scope)
         self.proxies = proxies
+        self.requests_timeout = requests_timeout
         self.show_dialog = show_dialog
 
     def get_cached_token(self):
         """ Gets a cached auth token
         """
         token_info = None
 
@@ -319,15 +325,15 @@
         print("")
         print("")
         return response
 
     def get_authorization_code(self, response=None):
         return self.parse_response_code(response or self.get_auth_response())
 
-    def get_access_token(self, code=None, as_dict=True):
+    def get_access_token(self, code=None, as_dict=True, check_cache=True):
         """ Gets the access token for the app given the code
 
             Parameters:
                 - code - the response code
                 - as_dict - a boolean indicating if returning the access token
                             as a token_info dictionary, otherwise it will be returned
                             as a string.
@@ -339,21 +345,22 @@
                 "get_access_token will return the token string directly in future "
                 "versions. Please adjust your code accordingly, or use "
                 "get_cached_token instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             print("")
-        token_info = self.get_cached_token()
-        if token_info is not None:
-            if is_token_expired(token_info):
-                token_info = self.refresh_access_token(
-                    token_info["refresh_token"]
-                )
-            return token_info if as_dict else token_info["access_token"]
+        if check_cache:
+            token_info = self.get_cached_token()
+            if token_info is not None:
+                if is_token_expired(token_info):
+                    token_info = self.refresh_access_token(
+                        token_info["refresh_token"]
+                    )
+                return token_info if as_dict else token_info["access_token"]
 
         payload = {
             "redirect_uri": self.redirect_uri,
             "code": code or self.get_authorization_code(),
             "grant_type": "authorization_code",
         }
         if self.scope:
@@ -365,14 +372,15 @@
 
         response = requests.post(
             self.OAUTH_TOKEN_URL,
             data=payload,
             headers=headers,
             verify=True,
             proxies=self.proxies,
+            timeout=self.requests_timeout,
         )
         if response.status_code != 200:
             raise SpotifyOauthError(response.reason)
         token_info = response.json()
         token_info = self._add_custom_values_to_token_info(token_info)
         self._save_token_info(token_info)
         return token_info if as_dict else token_info["access_token"]
@@ -393,14 +401,15 @@
         headers = self._make_authorization_headers()
 
         response = requests.post(
             self.OAUTH_TOKEN_URL,
             data=payload,
             headers=headers,
             proxies=self.proxies,
+            timeout=self.requests_timeout,
         )
         if response.status_code != 200:
             if False:  # debugging code
                 print("headers", headers)
                 print("request", response.url)
             self._warn(
                 "couldn't refresh token: code:%d reason:%s"
```

### Comparing `spotipy-2.8.0/spotipy/util.py` & `spotipy-2.9.0/spotipy/util.py`

 * *Files identical despite different names*

### Comparing `spotipy-2.8.0/spotipy.egg-info/PKG-INFO` & `spotipy-2.9.0/spotipy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy
-Version: 2.8.0
+Version: 2.9.0
 Summary: A light weight Python library for the Spotify Web API
 Home-page: http://spotipy.readthedocs.org/
 Author: @plamere
 Author-email: paul@echonest.com
 License: LICENSE.md
 Description: # Spotipy
         
@@ -26,15 +26,15 @@
         
         To get started, install spotipy and create an app on https://developers.spotify.com/.
         Add your new ID and SECRET to your environment:
         
             export SPOTIPY_CLIENT_ID=client_id_here
             export SPOTIPY_CLIENT_SECRET=client_secret_here
         
-            // on Windows, use `SET` instead of `export`).
+            // on Windows, use `SET` instead of `export`
         
         Then, create a Spotify object and call methods:
         
             import spotipy
             from spotipy.oauth2 import SpotifyClientCredentials
         
             sp = spotipy.Spotify(client_credentials_manager=SpotifyClientCredentials())
```

