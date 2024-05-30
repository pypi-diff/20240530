# Comparing `tmp/transmission_rpc-7.0.6.tar.gz` & `tmp/transmission_rpc-7.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-7.0.6.tar", max compression
+gzip compressed data, was "transmission_rpc-7.0.7a0.tar", max compression
```

## Comparing `transmission_rpc-7.0.6.tar` & `transmission_rpc-7.0.7a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1127 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/LICENSE
--rw-r--r--   0        0        0     2277 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/README.md
--rw-r--r--   0        0        0     2981 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/pyproject.toml
--rw-r--r--   0        0        0     2230 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    45797 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/client.py
--rw-r--r--   0        0        0    10069 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1640 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/error.py
--rw-r--r--   0        0        0        0 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/py.typed
--rw-r--r--   0        0        0    12505 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/session.py
--rw-r--r--   0        0        0    23775 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1873 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2024-05-18 17:20:25.511493 transmission_rpc-7.0.6/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3422 1970-01-01 00:00:00.000000 transmission_rpc-7.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1127 2024-05-30 17:26:51.879074 transmission_rpc-7.0.7a0/LICENSE
+-rw-r--r--   0        0        0     2277 2024-05-30 17:26:51.879074 transmission_rpc-7.0.7a0/README.md
+-rw-r--r--   0        0        0     3057 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0     2230 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    45352 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/client.py
+-rw-r--r--   0        0        0    10080 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1673 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/error.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/py.typed
+-rw-r--r--   0        0        0    12488 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23901 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1900 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2643 2024-05-30 17:26:51.883074 transmission_rpc-7.0.7a0/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 transmission_rpc-7.0.7a0/PKG-INFO
```

### Comparing `transmission_rpc-7.0.6/LICENSE` & `transmission_rpc-7.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.6/README.md` & `transmission_rpc-7.0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.6/pyproject.toml` & `transmission_rpc-7.0.7a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "7.0.6"
+version = "7.0.7a0"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
@@ -104,16 +104,21 @@
     "RUF",
     "SIM",
     "SLF",
     "TCH",
     "TID",
     "TRY",
     "YTT",
+    "UP",
+    "FA100",
+    "FA102"
 ]
 
+extend-fixable = ['UP']
+
 ignore = [
     'PLR0911',
     'INP001',
     'N806',
     'N802',
     'N803',
     'E501',
@@ -128,14 +133,15 @@
     'ISC003',
     'PLR0913',
     'RUF001',
     'SIM108',
     'TCH003',
     'RUF003',
     'RET504',
+    'TCH001',
     'TRY300',
     'TRY003',
     'TRY201',
     'TRY301',
     'PLR0912',
     'PLR0915',
     'PLR2004',
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/__init__.py` & `transmission_rpc-7.0.7a0/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-7.0.6/transmission_rpc/client.py` & `transmission_rpc-7.0.7a0/transmission_rpc/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from __future__ import annotations
+
 import json
 import logging
 import pathlib
 import string
 import time
 import types
-from typing import Any, BinaryIO, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, BinaryIO, Iterable, List, TypeVar, Union
 from urllib.parse import quote
 
 import requests
 import requests.auth
 import requests.exceptions
-from typing_extensions import Literal, TypedDict, deprecated
+from typing_extensions import Literal, Self, TypedDict, deprecated
 
 from transmission_rpc.constants import DEFAULT_TIMEOUT, LOGGER, RpcMethod
 from transmission_rpc.error import (
     TransmissionAuthError,
     TransmissionConnectError,
     TransmissionError,
     TransmissionTimeoutError,
@@ -34,38 +36,38 @@
 
 class ResponseData(TypedDict):
     arguments: Any
     tag: int
     result: str
 
 
-def ensure_location_str(s: Union[str, pathlib.Path]) -> str:
+def ensure_location_str(s: str | pathlib.Path) -> str:
     if isinstance(s, pathlib.Path):
         if s.is_absolute():
             return str(s)
 
         raise ValueError(
             "using relative `pathlib.Path` as remote path is not supported in v4.",
         )
 
     return str(s)
 
 
-def _parse_torrent_id(raw_torrent_id: Union[int, str]) -> Union[int, str]:
+def _parse_torrent_id(raw_torrent_id: int | str) -> int | str:
     if isinstance(raw_torrent_id, int):
         if raw_torrent_id >= 0:
             return raw_torrent_id
     elif isinstance(raw_torrent_id, str):
         if len(raw_torrent_id) != 40 or (set(raw_torrent_id) - set(valid_hash_char)):
             raise ValueError(f"torrent ids {raw_torrent_id} is not valid torrent id")
         return raw_torrent_id
     raise ValueError(f"{raw_torrent_id} is not valid torrent id")
 
 
-def _parse_torrent_ids(args: Any) -> Union[str, List[Union[str, int]]]:
+def _parse_torrent_ids(args: Any) -> str | list[str | int]:
     if args is None:
         return []
     if isinstance(args, int):
         return [_parse_torrent_id(args)]
     if isinstance(args, str):
         if args == "recently-active":
             return args
@@ -76,16 +78,16 @@
 
 
 class Client:
     def __init__(
         self,
         *,
         protocol: Literal["http", "https"] = "http",
-        username: Optional[str] = None,
-        password: Optional[str] = None,
+        username: str | None = None,
+        password: str | None = None,
         host: str = "127.0.0.1",
         port: int = 9091,
         path: str = "/transmission/rpc",
         timeout: float = DEFAULT_TIMEOUT,
         logger: logging.Logger = LOGGER,
     ):
         """
@@ -113,15 +115,15 @@
         auth = f"{username}{password}@" if (username or password) else ""
 
         if path == "/transmission/":
             path = "/transmission/rpc"
 
         url = f"{protocol}://{auth}{host}:{port}{path}"
         self._url = str(url)
-        self.__raw_session: Dict[str, Any] = {}
+        self.__raw_session: dict[str, Any] = {}
         self.__session_id = "0"
         self.__server_version: str = "(unknown)"
         self.__protocol_version: int = 17  # default 17
         self._http_session = requests.Session()
         self._http_session.trust_env = False
         self.__semver_version = None
         self.get_session()
@@ -130,20 +132,20 @@
     @property
     @deprecated("do not use internal property")
     def url(self) -> str:
         return self._url
 
     @property
     @deprecated("do not use internal property, use `get_torrent_arguments(rpc_version)` if you need")
-    def torrent_get_arguments(self) -> List[str]:
+    def torrent_get_arguments(self) -> list[str]:
         return self.__torrent_get_arguments
 
     @property
     @deprecated("do not use internal property, use `.get_session()` instead")
-    def raw_session(self) -> Dict[str, Any]:
+    def raw_session(self) -> dict[str, Any]:
         return self.__raw_session
 
     @property
     @deprecated("do not use internal property")
     def session_id(self) -> str:
         return self.__session_id
 
@@ -180,18 +182,18 @@
     def timeout(self) -> None:
         """
         Reset the HTTP query timeout to the default.
         """
         self._query_timeout = DEFAULT_TIMEOUT
 
     @property
-    def _http_header(self) -> Dict[str, str]:
+    def _http_header(self) -> dict[str, str]:
         return {_header_session_id: self.__session_id}
 
-    def _http_query(self, query: Dict[str, Any], timeout: Optional[_Timeout] = None) -> str:
+    def _http_query(self, query: dict[str, Any], timeout: _Timeout | None = None) -> str:
         """
         Query Transmission through HTTP.
         """
         request_count = 0
         if timeout is None:
             timeout = self.timeout
         while True:
@@ -229,19 +231,19 @@
 
             if r.status_code != 409:
                 return r.text
 
     def _request(
         self,
         method: RpcMethod,
-        arguments: Optional[Dict[str, Any]] = None,
-        ids: Optional[_TorrentIDs] = None,
+        arguments: dict[str, Any] | None = None,
+        ids: _TorrentIDs | None = None,
         require_ids: bool = False,
-        timeout: Optional[_Timeout] = None,
-    ) -> Dict[str, Any]:
+        timeout: _Timeout | None = None,
+    ) -> dict[str, Any]:
         """
         Send json-rpc request to Transmission using http POST
         """
         if not isinstance(method, str):
             raise TypeError("request takes method as string")
         if arguments is None:
             arguments = {}
@@ -336,15 +338,15 @@
         """Decode the Transmission version string, if available."""
         self.__semver_version = self.__raw_session.get("rpc-version-semver")
         self.__server_version = self.__raw_session["version"]
         self.__protocol_version = self.__raw_session["rpc-version"]
 
     @property
     @deprecated("use .get_session().rpc_version_semver instead")
-    def semver_version(self) -> Optional[int]:
+    def semver_version(self) -> int | None:
         """Get the Transmission daemon RPC version."""
         return self.__semver_version
 
     @property
     @deprecated("use .get_session().rpc_version instead")
     def rpc_version(self) -> int:
         """Get the Transmission daemon RPC version."""
@@ -359,28 +361,28 @@
                 "Using feature not supported by server. RPC version for server %d, feature introduced in %d.",
                 self.__protocol_version,
                 required_version,
             )
 
     def add_torrent(
         self,
-        torrent: Union[BinaryIO, str, bytes, pathlib.Path],
-        timeout: Optional[_Timeout] = None,
+        torrent: BinaryIO | str | bytes | pathlib.Path,
+        timeout: _Timeout | None = None,
         *,
-        download_dir: Optional[str] = None,
-        files_unwanted: Optional[List[int]] = None,
-        files_wanted: Optional[List[int]] = None,
-        paused: Optional[bool] = None,
-        peer_limit: Optional[int] = None,
-        priority_high: Optional[List[int]] = None,
-        priority_low: Optional[List[int]] = None,
-        priority_normal: Optional[List[int]] = None,
-        cookies: Optional[str] = None,
-        labels: Optional[Iterable[str]] = None,
-        bandwidthPriority: Optional[int] = None,
+        download_dir: str | None = None,
+        files_unwanted: list[int] | None = None,
+        files_wanted: list[int] | None = None,
+        paused: bool | None = None,
+        peer_limit: int | None = None,
+        priority_high: list[int] | None = None,
+        priority_low: list[int] | None = None,
+        priority_normal: list[int] | None = None,
+        cookies: str | None = None,
+        labels: Iterable[str] | None = None,
+        bandwidthPriority: int | None = None,
     ) -> Torrent:
         """
         Add torrent to transfers list. ``torrent`` can be:
 
         - ``http://``, ``https://`` or  ``magnet:`` URL
         - torrent file-like object in **binary mode**
         - bytes of torrent content
@@ -421,15 +423,15 @@
         """
         if torrent is None:
             raise ValueError("add_torrent requires data or a URI.")
 
         if labels is not None:
             self._rpc_version_warning(17)
 
-        kwargs: Dict[str, Any] = remove_unset_value(
+        kwargs: dict[str, Any] = remove_unset_value(
             {
                 "download-dir": download_dir,
                 "files-unwanted": files_unwanted,
                 "files-wanted": files_wanted,
                 "paused": paused,
                 "peer-limit": peer_limit,
                 "priority-high": priority_high,
@@ -445,66 +447,66 @@
         if torrent_data:
             kwargs["metainfo"] = torrent_data
         else:
             kwargs["filename"] = torrent
 
         return next(iter(self._request(RpcMethod.TorrentAdd, kwargs, timeout=timeout).values()))
 
-    def remove_torrent(self, ids: _TorrentIDs, delete_data: bool = False, timeout: Optional[_Timeout] = None) -> None:
+    def remove_torrent(self, ids: _TorrentIDs, delete_data: bool = False, timeout: _Timeout | None = None) -> None:
         """
         remove torrent(s) with provided id(s).
 
         Local data will be removed by transmission daemon if ``delete_data`` is set to ``True``.
         """
         self._request(
             RpcMethod.TorrentRemove,
             {"delete-local-data": delete_data},
             ids,
             True,
             timeout=timeout,
         )
 
-    def start_torrent(self, ids: _TorrentIDs, bypass_queue: bool = False, timeout: Optional[_Timeout] = None) -> None:
+    def start_torrent(self, ids: _TorrentIDs, bypass_queue: bool = False, timeout: _Timeout | None = None) -> None:
         """Start torrent(s) with provided id(s)"""
         method = RpcMethod.TorrentStart
         if bypass_queue:
             method = RpcMethod.TorrentStartNow
         self._request(method, {}, ids, True, timeout=timeout)
 
-    def start_all(self, bypass_queue: bool = False, timeout: Optional[_Timeout] = None) -> None:
+    def start_all(self, bypass_queue: bool = False, timeout: _Timeout | None = None) -> None:
         """Start all torrents respecting the queue order"""
         method = RpcMethod.TorrentStart
         if bypass_queue:
             method = RpcMethod.TorrentStartNow
         torrent_list = sorted(self.get_torrents(), key=lambda t: t.queue_position)
         self._request(
             method,
             {},
             ids=[x.id for x in torrent_list],
             require_ids=True,
             timeout=timeout,
         )
 
-    def stop_torrent(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def stop_torrent(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """stop torrent(s) with provided id(s)"""
         self._request(RpcMethod.TorrentStop, {}, ids, True, timeout=timeout)
 
-    def verify_torrent(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def verify_torrent(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """verify torrent(s) with provided id(s)"""
         self._request(RpcMethod.TorrentVerify, {}, ids, True, timeout=timeout)
 
-    def reannounce_torrent(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def reannounce_torrent(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """Reannounce torrent(s) with provided id(s)"""
         self._request(RpcMethod.TorrentReannounce, {}, ids, True, timeout=timeout)
 
     def get_torrent(
         self,
         torrent_id: _TorrentID,
-        arguments: Optional[Iterable[str]] = None,
-        timeout: Optional[_Timeout] = None,
+        arguments: Iterable[str] | None = None,
+        timeout: _Timeout | None = None,
     ) -> Torrent:
         """
         Get information for torrent with provided id.
         ``arguments`` contains a list of field names to be returned, when ``arguments=None`` (default),
         all fields are requested. See the Torrent class for more information.
 
         new argument ``format`` in rpc_version 16 is unnecessarily
@@ -552,18 +554,18 @@
         for torrent in result["torrents"]:
             if torrent.get("hashString") == torrent_id or torrent.get("id") == torrent_id:
                 return Torrent(fields=torrent)
         raise KeyError("Torrent not found in result")
 
     def get_torrents(
         self,
-        ids: Optional[_TorrentIDs] = None,
-        arguments: Optional[Iterable[str]] = None,
-        timeout: Optional[_Timeout] = None,
-    ) -> List[Torrent]:
+        ids: _TorrentIDs | None = None,
+        arguments: Iterable[str] | None = None,
+        timeout: _Timeout | None = None,
+    ) -> list[Torrent]:
         """
         Get information for torrents with provided ids. For more information see :py:meth:`Client.get_torrent`.
 
         Returns a list of Torrent object.
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
@@ -571,62 +573,62 @@
             arguments = self.__torrent_get_arguments
         return [
             Torrent(fields=x)
             for x in self._request(RpcMethod.TorrentGet, {"fields": arguments}, ids, timeout=timeout)["torrents"]
         ]
 
     def get_recently_active_torrents(
-        self, arguments: Optional[Iterable[str]] = None, timeout: Optional[_Timeout] = None
-    ) -> Tuple[List[Torrent], List[int]]:
+        self, arguments: Iterable[str] | None = None, timeout: _Timeout | None = None
+    ) -> tuple[list[Torrent], list[int]]:
         """
         Get information for torrents for recently active torrent. If you want to get recently-removed
         torrents. you should use this method.
 
         Returns:
             active_torrents, removed_torrents
-                List of recently active torrents and list of torrent-id of recently-removed torrents.
+                list of recently active torrents and list of torrent-id of recently-removed torrents.
         """
         if arguments:
             arguments = list(set(arguments) | {"id", "hashString"})
         else:
             arguments = self.__torrent_get_arguments
 
         result = self._request(RpcMethod.TorrentGet, {"fields": arguments}, "recently-active", timeout=timeout)
 
         return [Torrent(fields=x) for x in result["torrents"]], result["removed"]
 
     def change_torrent(
         self,
         ids: _TorrentIDs,
-        timeout: Optional[_Timeout] = None,
+        timeout: _Timeout | None = None,
         *,
-        bandwidth_priority: Optional[int] = None,
-        download_limit: Optional[int] = None,
-        download_limited: Optional[bool] = None,
-        upload_limit: Optional[int] = None,
-        upload_limited: Optional[bool] = None,
-        files_unwanted: Optional[Iterable[int]] = None,
-        files_wanted: Optional[Iterable[int]] = None,
-        honors_session_limits: Optional[bool] = None,
-        location: Optional[str] = None,
-        peer_limit: Optional[int] = None,
-        priority_high: Optional[Iterable[int]] = None,
-        priority_low: Optional[Iterable[int]] = None,
-        priority_normal: Optional[Iterable[int]] = None,
-        queue_position: Optional[int] = None,
-        seed_idle_limit: Optional[int] = None,
-        seed_idle_mode: Optional[int] = None,
-        seed_ratio_limit: Optional[float] = None,
-        seed_ratio_mode: Optional[int] = None,
-        tracker_add: Optional[Iterable[str]] = None,
-        labels: Optional[Iterable[str]] = None,
-        group: Optional[str] = None,
-        tracker_list: Optional[Iterable[Iterable[str]]] = None,
-        tracker_replace: Optional[Iterable[Tuple[int, str]]] = None,
-        tracker_remove: Optional[Iterable[int]] = None,
+        bandwidth_priority: int | None = None,
+        download_limit: int | None = None,
+        download_limited: bool | None = None,
+        upload_limit: int | None = None,
+        upload_limited: bool | None = None,
+        files_unwanted: Iterable[int] | None = None,
+        files_wanted: Iterable[int] | None = None,
+        honors_session_limits: bool | None = None,
+        location: str | None = None,
+        peer_limit: int | None = None,
+        priority_high: Iterable[int] | None = None,
+        priority_low: Iterable[int] | None = None,
+        priority_normal: Iterable[int] | None = None,
+        queue_position: int | None = None,
+        seed_idle_limit: int | None = None,
+        seed_idle_mode: int | None = None,
+        seed_ratio_limit: float | None = None,
+        seed_ratio_mode: int | None = None,
+        tracker_add: Iterable[str] | None = None,
+        labels: Iterable[str] | None = None,
+        group: str | None = None,
+        tracker_list: Iterable[Iterable[str]] | None = None,
+        tracker_replace: Iterable[tuple[int, str]] | None = None,
+        tracker_remove: Iterable[int] | None = None,
         **kwargs: Any,
     ) -> None:
         """Change torrent parameters for the torrent(s) with the supplied id's.
 
         Parameters:
             ids: torrent(s) to change.
             timeout: requesst timeout.
@@ -687,15 +689,15 @@
 
         if tracker_list is not None:
             self._rpc_version_warning(17)
 
         if group is not None:
             self._rpc_version_warning(17)
 
-        args: Dict[str, Any] = remove_unset_value(
+        args: dict[str, Any] = remove_unset_value(
             {
                 "bandwidthPriority": bandwidth_priority,
                 "downloadLimit": download_limit,
                 "downloadLimited": download_limited,
                 "uploadLimit": upload_limit,
                 "uploadLimited": upload_limited,
                 "files-unwanted": list_or_none(files_unwanted),
@@ -711,31 +713,31 @@
                 "seedIdleMode": seed_idle_mode,
                 "seedRatioLimit": seed_ratio_limit,
                 "seedRatioMode": seed_ratio_mode,
                 "trackerAdd": tracker_add,
                 "trackerRemove": tracker_remove,
                 "trackerReplace": tracker_replace,
                 "labels": list_or_none(_single_str_as_list(labels)),
-                "trackerList": None if tracker_list is None else "\n".join("\n\n".join(x) for x in tracker_list),
+                "trackerlist": None if tracker_list is None else "\n".join("\n\n".join(x) for x in tracker_list),
                 "group": group,
             }
         )
 
         args.update(kwargs)
 
         if args:
             self._request(RpcMethod.TorrentSet, args, ids, True, timeout=timeout)
         else:
             ValueError("No arguments to set")
 
     def move_torrent_data(
         self,
         ids: _TorrentIDs,
-        location: Union[str, pathlib.Path],
-        timeout: Optional[_Timeout] = None,
+        location: str | pathlib.Path,
+        timeout: _Timeout | None = None,
         *,
         move: bool = True,
     ) -> None:
         """
         Move torrent data to the new location.
 
         See Also:
@@ -745,16 +747,16 @@
         self._request(RpcMethod.TorrentSetLocation, args, ids, True, timeout=timeout)
 
     def rename_torrent_path(
         self,
         torrent_id: _TorrentID,
         location: str,
         name: str,
-        timeout: Optional[_Timeout] = None,
-    ) -> Tuple[str, str]:
+        timeout: _Timeout | None = None,
+    ) -> tuple[str, str]:
         """
         Warnings:
             This method can only be called on single torrent.
 
         Warnings:
             This is not the method to move torrent data directory,
 
@@ -772,97 +774,97 @@
             torrent_id,
             True,
             timeout=timeout,
         )
 
         return result["path"], result["name"]
 
-    def queue_top(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def queue_top(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """
         Move transfer to the top of the queue.
 
         https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#46-queue-movement-requests
         """
         self._request(RpcMethod.QueueMoveTop, ids=ids, require_ids=True, timeout=timeout)
 
-    def queue_bottom(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def queue_bottom(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """
         Move transfer to the bottom of the queue.
 
         https://github.com/transmission/transmission/blob/main/docs/rpc-spec.md#46-queue-movement-requests
         """
         self._request(RpcMethod.QueueMoveBottom, ids=ids, require_ids=True, timeout=timeout)
 
-    def queue_up(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def queue_up(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """Move transfer up in the queue."""
         self._request(RpcMethod.QueueMoveUp, ids=ids, require_ids=True, timeout=timeout)
 
-    def queue_down(self, ids: _TorrentIDs, timeout: Optional[_Timeout] = None) -> None:
+    def queue_down(self, ids: _TorrentIDs, timeout: _Timeout | None = None) -> None:
         """Move transfer down in the queue."""
         self._request(RpcMethod.QueueMoveDown, ids=ids, require_ids=True, timeout=timeout)
 
-    def get_session(self, timeout: Optional[_Timeout] = None) -> Session:
+    def get_session(self, timeout: _Timeout | None = None) -> Session:
         """
         Get session parameters. See the Session class for more information.
         """
         self._request(RpcMethod.SessionGet, timeout=timeout)
         self._update_server_version()
         return Session(fields=self.__raw_session)
 
     def set_session(
         self,
-        timeout: Optional[_Timeout] = None,
+        timeout: _Timeout | None = None,
         *,
-        alt_speed_down: Optional[int] = None,
-        alt_speed_enabled: Optional[bool] = None,
-        alt_speed_time_begin: Optional[int] = None,
-        alt_speed_time_day: Optional[int] = None,
-        alt_speed_time_enabled: Optional[bool] = None,
-        alt_speed_time_end: Optional[int] = None,
-        alt_speed_up: Optional[int] = None,
-        blocklist_enabled: Optional[bool] = None,
-        blocklist_url: Optional[str] = None,
-        cache_size_mb: Optional[int] = None,
-        dht_enabled: Optional[bool] = None,
-        default_trackers: Optional[Iterable[str]] = None,
-        download_dir: Optional[str] = None,
-        download_queue_enabled: Optional[bool] = None,
-        download_queue_size: Optional[int] = None,
-        encryption: Optional[Literal["required", "preferred", "tolerated"]] = None,
-        idle_seeding_limit: Optional[int] = None,
-        idle_seeding_limit_enabled: Optional[bool] = None,
-        incomplete_dir: Optional[str] = None,
-        incomplete_dir_enabled: Optional[bool] = None,
-        lpd_enabled: Optional[bool] = None,
-        peer_limit_global: Optional[int] = None,
-        peer_limit_per_torrent: Optional[int] = None,
-        peer_port: Optional[int] = None,
-        peer_port_random_on_start: Optional[bool] = None,
-        pex_enabled: Optional[bool] = None,
-        port_forwarding_enabled: Optional[bool] = None,
-        queue_stalled_enabled: Optional[bool] = None,
-        queue_stalled_minutes: Optional[int] = None,
-        rename_partial_files: Optional[bool] = None,
-        script_torrent_done_enabled: Optional[bool] = None,
-        script_torrent_done_filename: Optional[str] = None,
-        seed_queue_enabled: Optional[bool] = None,
-        seed_queue_size: Optional[int] = None,
-        seed_ratio_limit: Optional[int] = None,
-        seed_ratio_limited: Optional[bool] = None,
-        speed_limit_down: Optional[int] = None,
-        speed_limit_down_enabled: Optional[bool] = None,
-        speed_limit_up: Optional[int] = None,
-        speed_limit_up_enabled: Optional[bool] = None,
-        start_added_torrents: Optional[bool] = None,
-        trash_original_torrent_files: Optional[bool] = None,
-        utp_enabled: Optional[bool] = None,
-        script_torrent_done_seeding_filename: Optional[str] = None,
-        script_torrent_done_seeding_enabled: Optional[bool] = None,
-        script_torrent_added_enabled: Optional[bool] = None,
-        script_torrent_added_filename: Optional[str] = None,
+        alt_speed_down: int | None = None,
+        alt_speed_enabled: bool | None = None,
+        alt_speed_time_begin: int | None = None,
+        alt_speed_time_day: int | None = None,
+        alt_speed_time_enabled: bool | None = None,
+        alt_speed_time_end: int | None = None,
+        alt_speed_up: int | None = None,
+        blocklist_enabled: bool | None = None,
+        blocklist_url: str | None = None,
+        cache_size_mb: int | None = None,
+        dht_enabled: bool | None = None,
+        default_trackers: Iterable[str] | None = None,
+        download_dir: str | None = None,
+        download_queue_enabled: bool | None = None,
+        download_queue_size: int | None = None,
+        encryption: Literal["required", "preferred", "tolerated"] | None = None,
+        idle_seeding_limit: int | None = None,
+        idle_seeding_limit_enabled: bool | None = None,
+        incomplete_dir: str | None = None,
+        incomplete_dir_enabled: bool | None = None,
+        lpd_enabled: bool | None = None,
+        peer_limit_global: int | None = None,
+        peer_limit_per_torrent: int | None = None,
+        peer_port: int | None = None,
+        peer_port_random_on_start: bool | None = None,
+        pex_enabled: bool | None = None,
+        port_forwarding_enabled: bool | None = None,
+        queue_stalled_enabled: bool | None = None,
+        queue_stalled_minutes: int | None = None,
+        rename_partial_files: bool | None = None,
+        script_torrent_done_enabled: bool | None = None,
+        script_torrent_done_filename: str | None = None,
+        seed_queue_enabled: bool | None = None,
+        seed_queue_size: int | None = None,
+        seed_ratio_limit: int | None = None,
+        seed_ratio_limited: bool | None = None,
+        speed_limit_down: int | None = None,
+        speed_limit_down_enabled: bool | None = None,
+        speed_limit_up: int | None = None,
+        speed_limit_up_enabled: bool | None = None,
+        start_added_torrents: bool | None = None,
+        trash_original_torrent_files: bool | None = None,
+        utp_enabled: bool | None = None,
+        script_torrent_done_seeding_filename: str | None = None,
+        script_torrent_done_seeding_enabled: bool | None = None,
+        script_torrent_added_enabled: bool | None = None,
+        script_torrent_added_filename: str | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Set session parameters.
 
         Parameters:
             timeout
@@ -884,15 +886,15 @@
             blocklist_enabled:
                 Enables the block list
             blocklist_url:
                 Location of the block list. Updated with blocklist-update.
             cache_size_mb:
                 The maximum size of the disk cache in MB
             default_trackers:
-                List of default trackers to use on public torrents.
+                list of default trackers to use on public torrents.
             dht_enabled:
                 Enables DHT.
             download_dir:
                 Set the session download directory.
             download_queue_enabled:
                 Enables download queue.
             download_queue_size:
@@ -979,15 +981,15 @@
         if script_torrent_done_seeding_enabled is not None:
             self._rpc_version_warning(17)
         if script_torrent_added_enabled is not None:
             self._rpc_version_warning(17)
         if script_torrent_added_filename is not None:
             self._rpc_version_warning(17)
 
-        args: Dict[str, Any] = remove_unset_value(
+        args: dict[str, Any] = remove_unset_value(
             {
                 "alt-speed-down": alt_speed_down,
                 "alt-speed-enabled": alt_speed_enabled,
                 "alt-speed-time-begin": alt_speed_time_begin,
                 "alt-speed-time-day": alt_speed_time_day,
                 "alt-speed-time-enabled": alt_speed_time_enabled,
                 "alt-speed-time-end": alt_speed_time_end,
@@ -1036,121 +1038,121 @@
         )
 
         args.update(kwargs)
 
         if args:
             self._request(RpcMethod.SessionSet, args, timeout=timeout)
 
-    def blocklist_update(self, timeout: Optional[_Timeout] = None) -> Optional[int]:
+    def blocklist_update(self, timeout: _Timeout | None = None) -> int | None:
         """Update block list. Returns the size of the block list."""
         result = self._request(RpcMethod.BlocklistUpdate, timeout=timeout)
         return result.get("blocklist-size")
 
-    def port_test(self, timeout: Optional[_Timeout] = None) -> Optional[bool]:
+    def port_test(self, timeout: _Timeout | None = None) -> bool | None:
         """
         Tests to see if your incoming peer port is accessible from the
         outside world.
         """
         result = self._request(RpcMethod.PortTest, timeout=timeout)
         return result.get("port-is-open")
 
-    def free_space(self, path: Union[str, pathlib.Path], timeout: Optional[_Timeout] = None) -> Optional[int]:
+    def free_space(self, path: str | pathlib.Path, timeout: _Timeout | None = None) -> int | None:
         """
         Get the amount of free space (in bytes) at the provided location.
         """
         self._rpc_version_warning(15)
         path = ensure_location_str(path)
-        result: Dict[str, Any] = self._request(RpcMethod.FreeSpace, {"path": path}, timeout=timeout)
+        result: dict[str, Any] = self._request(RpcMethod.FreeSpace, {"path": path}, timeout=timeout)
         if result["path"] == path:
             return result["size-bytes"]
         return None
 
-    def session_stats(self, timeout: Optional[_Timeout] = None) -> SessionStats:
+    def session_stats(self, timeout: _Timeout | None = None) -> SessionStats:
         """Get session statistics"""
         result = self._request(RpcMethod.SessionStats, timeout=timeout)
         return SessionStats(fields=result)
 
     def set_group(
         self,
         name: str,
         *,
-        timeout: Optional[_Timeout] = None,
-        honors_session_limits: Optional[bool] = None,
-        speed_limit_down_enabled: Optional[bool] = None,
-        speed_limit_down: Optional[int] = None,
-        speed_limit_up_enabled: Optional[bool] = None,
-        speed_limit_up: Optional[int] = None,
+        timeout: _Timeout | None = None,
+        honors_session_limits: bool | None = None,
+        speed_limit_down_enabled: bool | None = None,
+        speed_limit_down: int | None = None,
+        speed_limit_up_enabled: bool | None = None,
+        speed_limit_up: int | None = None,
     ) -> None:
         """create or update a Bandwidth group.
 
         :param name: Bandwidth group name
         :param honors_session_limits: true if session upload limits are honored
         :param speed_limit_down_enabled: true means enabled
         :param speed_limit_down: 	max global download speed (KBps)
         :param speed_limit_up_enabled: 	true means enabled
         :param speed_limit_up: max global upload speed (KBps)
         :param timeout: request timeout
         """
 
         self._rpc_version_warning(17)
-        arguments: Dict[str, Any] = remove_unset_value(
+        arguments: dict[str, Any] = remove_unset_value(
             {
                 "name": name,
                 "honorsSessionLimits": honors_session_limits,
                 "speed-limit-down": speed_limit_down,
                 "speed-limit-up-enabled": speed_limit_up_enabled,
                 "speed-limit-up": speed_limit_up,
                 "speed-limit-down-enabled": speed_limit_down_enabled,
             }
         )
 
         self._request(RpcMethod.GroupSet, arguments, timeout=timeout)
 
-    def get_group(self, name: str, *, timeout: Optional[_Timeout] = None) -> Optional[Group]:
+    def get_group(self, name: str, *, timeout: _Timeout | None = None) -> Group | None:
         self._rpc_version_warning(17)
-        result: Dict[str, Any] = self._request(RpcMethod.GroupGet, {"group": name}, timeout=timeout)
+        result: dict[str, Any] = self._request(RpcMethod.GroupGet, {"group": name}, timeout=timeout)
 
         if result["group"]:
             return Group(fields=result["group"][0])
 
         return None
 
-    def get_groups(self, name: Optional[List[str]] = None, *, timeout: Optional[_Timeout] = None) -> Dict[str, Group]:
+    def get_groups(self, name: list[str] | None = None, *, timeout: _Timeout | None = None) -> dict[str, Group]:
         payload = {}
         if name is not None:
             payload = {"group": name}
 
-        result: Dict[str, Any] = self._request(RpcMethod.GroupGet, payload, timeout=timeout)
+        result: dict[str, Any] = self._request(RpcMethod.GroupGet, payload, timeout=timeout)
 
         return {x["name"]: Group(fields=x) for x in result["group"]}
 
-    def __enter__(self) -> "Client":
+    def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[types.TracebackType],
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: types.TracebackType | None,
     ) -> None:
         self._http_session.close()
 
 
 T = TypeVar("T")
 
 
-def _single_str_as_list(v: Optional[Iterable[str]]) -> Optional[List[str]]:
+def _single_str_as_list(v: Iterable[str] | None) -> list[str] | None:
     if v is None:
         return v
     if isinstance(v, str):
         return [v]
     return list(v)
 
 
-def list_or_none(v: Optional[Iterable[T]]) -> Optional[List[T]]:
+def list_or_none(v: Iterable[T] | None) -> list[T] | None:
     if v is None:
         return None
     return list(v)
 
 
-def remove_unset_value(data: Dict[str, Any]) -> Dict[str, Any]:
+def remove_unset_value(data: dict[str, Any]) -> dict[str, Any]:
     return {key: value for key, value in data.items() if value is not None}
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/constants.py` & `transmission_rpc-7.0.7a0/transmission_rpc/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) 2018-2022 Trim21 <i@trim21.me>
 # Copyright (c) 2008-2014 Erik Svensson <erik.public@gmail.com>
 # Licensed under the MIT license.
+from __future__ import annotations
+
 import enum
 import logging
-from typing import Dict, NamedTuple, Optional
+from typing import NamedTuple
 
 LOGGER = logging.getLogger("transmission-rpc")
 LOGGER.setLevel(logging.ERROR)
 
 
 DEFAULT_TIMEOUT = 30.0
 
@@ -39,17 +41,17 @@
     #: override the global settings, seeding regardless of activity
     Unlimited = 2
 
 
 class Args(NamedTuple):
     type: str
     added_version: int
-    removed_version: Optional[int] = None
-    previous_argument_name: Optional[str] = None
-    next_argument_name: Optional[str] = None
+    removed_version: int | None = None
+    previous_argument_name: str | None = None
+    next_argument_name: str | None = None
     description: str = ""
 
     def __repr__(self) -> str:
         return (
             f"Args({self.type!r},"
             f" {self.added_version!r},"
             f" {self.removed_version!r},"
@@ -67,15 +69,15 @@
     string = "string"
     array = "array"
     boolean = "boolean"
     double = "double"
     object = "object"
 
 
-TORRENT_GET_ARGS: Dict[str, Args] = {
+TORRENT_GET_ARGS: dict[str, Args] = {
     "activityDate": Args(Type.number, 1, description="Last time of upload or download activity."),
     "addedDate": Args(Type.number, 1, description="The date when this torrent was first added."),
     "bandwidthPriority": Args(Type.number, 5, description="Bandwidth priority. Low (-1), Normal (0) or High (1)."),
     "comment": Args(Type.string, 1, description="Torrent comment."),
     "corruptEver": Args(Type.number, 1, description="Number of bytes of corrupt data downloaded."),
     "creator": Args(Type.string, 1, description="Torrent creator."),
     "dateCreated": Args(Type.number, 1, description="Torrent creation date."),
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/error.py` & `transmission_rpc-7.0.7a0/transmission_rpc/error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """
 exception raise by this package
 """
 
-from typing import Any, Optional
+from __future__ import annotations
 
-from requests.models import Response
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from requests.models import Response
 
 
 class TransmissionError(Exception):
     """
     This exception is raised when there has occurred an error related to
     communication with Transmission.
     """
 
     message: str
-    method: Optional[Any]  # rpc call method
-    argument: Optional[Any]  # rpc call arguments
-    response: Optional[Any]  # parsed json response, may be dict with keys 'result' and 'arguments'
-    rawResponse: Optional[str]  # raw text http response
-    original: Optional[Response]  # original http requests
+    method: Any | None  # rpc call method
+    argument: Any | None  # rpc call arguments
+    response: Any | None  # parsed json response, may be dict with keys 'result' and 'arguments'
+    rawResponse: str | None  # raw text http response
+    original: Response | None  # original http requests
 
     def __init__(
         self,
         message: str = "",
-        method: Optional[Any] = None,
-        argument: Optional[Any] = None,
-        response: Optional[Any] = None,
-        rawResponse: Optional[str] = None,
-        original: Optional[Response] = None,
+        method: Any | None = None,
+        argument: Any | None = None,
+        response: Any | None = None,
+        rawResponse: str | None = None,
+        original: Response | None = None,
     ):
         super().__init__()
         self.message = message
         self.method = method
         self.argument = argument
         self.response = response
         self.rawResponse = rawResponse
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/session.py` & `transmission_rpc-7.0.7a0/transmission_rpc/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from __future__ import annotations
 
 from typing_extensions import Literal
 
 from transmission_rpc.types import Container
 
 
 class Stats(Container):
@@ -59,35 +59,35 @@
     def current_stats(self) -> Stats:
         return Stats(fields=self.fields["current-stats"])
 
 
 class Units(Container):
     # 4 strings: KB/s, MB/s, GB/s, TB/s
     @property
-    def speed_units(self) -> List[str]:
+    def speed_units(self) -> list[str]:
         return self.fields["speed-units"]
 
     # number of bytes in a KB (1000 for kB; 1024 for KiB)
     @property
     def speed_bytes(self) -> int:
         return self.fields["speed-bytes"]
 
     # 4 strings: KB/s, MB/s, GB/s, TB/s
     @property
-    def size_units(self) -> List[str]:
+    def size_units(self) -> list[str]:
         return self.fields["size-units"]
 
     # number of bytes in a KB (1000 for kB; 1024 for KiB)
     @property
     def size_bytes(self) -> int:
         return self.fields["size-bytes"]
 
     # 4 strings: KB/s, MB/s, GB/s, TB/s
     @property
-    def memory_units(self) -> List[str]:
+    def memory_units(self) -> list[str]:
         return self.fields["memory-units"]
 
     # number of bytes in a KB (1000 for kB; 1024 for KiB)
     @property
     def memory_bytes(self) -> int:
         return self.fields["memory-bytes"]
 
@@ -356,56 +356,56 @@
 
     @property
     def version(self) -> str:
         """long version str `$version ($revision)`"""
         return self.fields["version"]
 
     @property
-    def default_trackers(self) -> Optional[List[str]]:
+    def default_trackers(self) -> list[str] | None:
         """
         list of default trackers to use on public torrents
         new at rpc-version 17
         """
         trackers = self.get("default-trackers")
         if trackers:
             return trackers.split("\n")
         return None
 
     @property
-    def rpc_version_semver(self) -> Optional[str]:
+    def rpc_version_semver(self) -> str | None:
         """
         the current RPC API version in a semver-compatible str
         new at rpc-version 17
         """
         return self.get("rpc-version-semver")
 
     @property
-    def script_torrent_added_enabled(self) -> Optional[bool]:
+    def script_torrent_added_enabled(self) -> bool | None:
         """
         whether to call the `added` script
         new at rpc-version 17
         """
         return self.get("script-torrent-added-enabled")
 
     @property
-    def script_torrent_added_filename(self) -> Optional[str]:
+    def script_torrent_added_filename(self) -> str | None:
         """
         filename of the script to run
         new at rpc-version 17
         """
         return self.get("script-torrent-added-filename")
 
     @property
-    def script_torrent_done_seeding_enabled(self) -> Optional[bool]:
+    def script_torrent_done_seeding_enabled(self) -> bool | None:
         """
         whether to call the `seeding-done` script
         new at rpc-version 17
         """
         return self.get("script-torrent-done-seeding-enabled")
 
     @property
-    def script_torrent_done_seeding_filename(self) -> Optional[str]:
+    def script_torrent_done_seeding_filename(self) -> str | None:
         """
         filename of the script to run
         new at rpc-version 17
         """
         return self.get("script-torrent-done-seeding-filename")
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/torrent.py` & `transmission_rpc-7.0.7a0/transmission_rpc/torrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import enum
 from datetime import datetime, timedelta, timezone
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 from transmission_rpc.constants import IdleMode, Priority, RatioLimitMode
 from transmission_rpc.types import Container, File
 from transmission_rpc.utils import format_timedelta
 
 _STATUS_NEW_MAPPING = {
     0: "stopped",
@@ -22,20 +24,31 @@
     return _STATUS_NEW_MAPPING.get(code) or f"unknown status {code}"
 
 
 class Status(str, enum.Enum):
     """enum for torrent status"""
 
     STOPPED = "stopped"
+    """"""
     CHECK_PENDING = "check pending"
+    """"""
+
     CHECKING = "checking"
+    """"""
     DOWNLOAD_PENDING = "download pending"
+    """"""
+
     DOWNLOADING = "downloading"
+    """"""
+
     SEED_PENDING = "seed pending"
+    """"""
+
     SEEDING = "seeding"
+    """"""
 
     @property
     def stopped(self) -> bool:
         """if torrent stopped"""
         return self == "stopped"
 
     @property
@@ -230,15 +243,15 @@
     """
     Torrent is a class holding the data received from Transmission regarding a bittorrent transfer.
 
     Warnings:
         setter on Torrent's properties has been removed, please use :py:meth:`Client.change_torrent` instead
     """
 
-    def __init__(self, *, fields: Dict[str, Any]):
+    def __init__(self, *, fields: dict[str, Any]):
         if "id" not in fields:
             raise ValueError(
                 "Torrent object requires field 'id', "
                 "you need to add 'id' in your 'arguments' when calling 'get_torrent'"
             )
 
         super().__init__(fields=fields)
@@ -346,15 +359,15 @@
 
     @property
     def error_string(self) -> str:
         """empty string for fine task"""
         return self.fields["errorString"]
 
     @property
-    def eta(self) -> Optional[timedelta]:
+    def eta(self) -> timedelta | None:
         """
         the "eta" as datetime.timedelta.
 
         If downloading, estimated the ``timedelta`` left until the torrent is done.
         If seeding, estimated the ``timedelta`` left until seed ratio is reached.
 
         raw `eta` maybe negative:
@@ -366,25 +379,25 @@
         eta = self.fields["eta"]
         if eta >= 0:
             return timedelta(seconds=eta)
 
         return None
 
     @property
-    def eta_idle(self) -> Optional[timedelta]:
+    def eta_idle(self) -> timedelta | None:
         v = self.fields["etaIdle"]
         if v >= 0:
             return timedelta(seconds=v)
         return None
 
     @property
-    def file_count(self) -> Optional[int]:
+    def file_count(self) -> int | None:
         return self.fields["file-count"]
 
-    def get_files(self) -> List[File]:
+    def get_files(self) -> list[File]:
         """
         Get list of files for this torrent.
 
         Note:
             The order of the files is guaranteed. The index of file object is the id of the file
             when calling :py:meth:`transmission_rpc.Client.change_torrent`
 
@@ -394,15 +407,15 @@
 
             torrent = Client().get_torrent(0)
 
             for file in torrent.get_files():
                 print(file.id)
 
         """
-        result: List[File] = []
+        result: list[File] = []
         if "files" in self.fields:
             files = self.fields["files"]
             indices = range(len(files))
             priorities = self.fields["priorities"]
             wanted = self.fields["wanted"]
             result.extend(
                 File(
@@ -415,15 +428,15 @@
                 )
                 for id, file, raw_priority, raw_selected in zip(indices, files, priorities, wanted)
             )
 
         return result
 
     @property
-    def file_stats(self) -> List[FileStat]:
+    def file_stats(self) -> list[FileStat]:
         """file stats"""
         return [FileStat(fields=x) for x in self.fields["fileStats"]]
 
     @property
     def group(self) -> str:
         return self.get("group", "")
 
@@ -455,15 +468,15 @@
         return self.fields["isPrivate"]
 
     @property
     def is_stalled(self) -> bool:
         return self.fields["isStalled"]
 
     @property
-    def labels(self) -> List[str]:
+    def labels(self) -> list[str]:
         return self.fields["labels"]
 
     @property
     def left_until_done(self) -> int:
         """
         Byte count of how much data is left to be downloaded until we've got
         all the pieces that we want. [0...tr_stat.sizeWhenDone]
@@ -600,25 +613,25 @@
     #     return self.fields["seedIdleMode"]
 
     @property
     def size_when_done(self) -> int:
         return self.fields["sizeWhenDone"]
 
     @property
-    def trackers(self) -> List[Tracker]:
+    def trackers(self) -> list[Tracker]:
         """trackers of torrent"""
         return [Tracker(fields=x) for x in self.fields["trackers"]]
 
     @property
-    def tracker_list(self) -> List[str]:
+    def tracker_list(self) -> list[str]:
         """list of str of announce URLs"""
-        return [x for x in self.fields["trackerList"].splitlines() if x]
+        return [x for x in self.fields["trackerlist"].splitlines() if x]
 
     @property
-    def tracker_stats(self) -> List[TrackerStats]:
+    def tracker_stats(self) -> list[TrackerStats]:
         """tracker status, for example, announce success/failure status"""
         return [TrackerStats(fields=x) for x in self.fields["trackerStats"]]
 
     @property
     def total_size(self) -> int:
         return self.fields["totalSize"]
 
@@ -646,20 +659,20 @@
         return self.fields["uploadLimited"]
 
     @property
     def upload_ratio(self) -> float:
         return self.fields["uploadRatio"]
 
     @property
-    def wanted(self) -> List[int]:
+    def wanted(self) -> list[int]:
         """if files are wanted, sorted by file index. 1 for wanted 0 for unwanted"""
         return self.fields["wanted"]
 
     @property
-    def webseeds(self) -> List[str]:
+    def webseeds(self) -> list[str]:
         return self.fields["webseeds"]
 
     @property
     def webseeds_sending_to_us(self) -> int:
         """Number of webseeds that are sending data to us."""
         return self.fields["webseedsSendingToUs"]
 
@@ -763,15 +776,15 @@
 
     @property
     def start_date(self) -> datetime:
         """raw field ``startDate`` as ``datetime.datetime`` in **utc timezone**."""
         return datetime.fromtimestamp(self.fields["startDate"], timezone.utc)
 
     @property
-    def done_date(self) -> Optional[datetime]:
+    def done_date(self) -> datetime | None:
         """the attribute "doneDate" as datetime.datetime. returns None if "doneDate" is invalid."""
         done_date = self.fields["doneDate"]
         # Transmission might forget to set doneDate which is initialized to zero,
         # so if doneDate is zero return None
         if done_date == 0:
             return None
         return datetime.fromtimestamp(done_date).astimezone()
@@ -838,11 +851,11 @@
          * global, use session seed ratio limit.
          * single, use torrent seed ratio limit. See seed_ratio_limit.
          * unlimited, no seed ratio limit.
         """
         return RatioLimitMode(self.fields["seedRatioMode"])
 
     def __repr__(self) -> str:
-        return f'<Torrent {self.id} "{self.name}">'
+        return f"<transmission_rpc.Torrent hashString={self.hashString!r}>"
 
     def __str__(self) -> str:
-        return f'Torrent "{self.name}"'
+        return f"<transmission_rpc.Torrent {self.name!r}>"
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/types.py` & `transmission_rpc-7.0.7a0/transmission_rpc/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from typing import Any, Dict, NamedTuple, Optional, Tuple, TypeVar, Union
+from __future__ import annotations
+
+from typing import Any, NamedTuple, Optional, Tuple, TypeVar, Union
 
 from transmission_rpc.constants import Priority
 
 _Number = Union[int, float]
 _Timeout = Optional[Union[_Number, Tuple[_Number, _Number]]]
 
 T = TypeVar("T")
 
 
 class Container:
-    fields: Dict[str, Any]  #: raw response data
+    fields: dict[str, Any]  #: raw response data
 
-    def __init__(self, *, fields: Dict[str, Any]):
+    def __init__(self, *, fields: dict[str, Any]):
         self.fields = fields
 
-    def get(self, key: str, default: Optional[T] = None) -> Any:
+    def get(self, key: str, default: T | None = None) -> Any:
         """get the raw value by the **raw rpc response key**"""
         return self.fields.get(key, default)
 
 
 class File(NamedTuple):
     name: str  # file name
     size: int  # file size in bytes
```

### Comparing `transmission_rpc-7.0.6/transmission_rpc/utils.py` & `transmission_rpc-7.0.7a0/transmission_rpc/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Copyright (c) 2018-2021 Trim21 <i@trim21.me>
 # Copyright (c) 2008-2014 Erik Svensson <erik.public@gmail.com>
 # Licensed under the MIT license.
+from __future__ import annotations
+
 import base64
 import datetime
 import pathlib
-from typing import BinaryIO, List, Optional, Tuple, Union
+from typing import BinaryIO
 from urllib.parse import urlparse
 
 from transmission_rpc import constants
 
 UNITS = ["B", "KiB", "MiB", "GiB", "TiB", "PiB", "EiB"]
 
 
-def format_size(size: int) -> Tuple[float, str]:
+def format_size(size: int) -> tuple[float, str]:
     """
     Format byte size into IEC prefixes, B, KiB, MiB ...
     """
     s = float(size)
     i = 0
     while s >= 1024.0 and i < len(UNITS):
         i += 1
         s /= 1024.0
     return s, UNITS[i]
 
 
-def format_speed(size: int) -> Tuple[float, str]:
+def format_speed(size: int) -> tuple[float, str]:
     """
     Format bytes per second speed into IEC prefixes, B/s, KiB/s, MiB/s ...
     """
     (s, unit) = format_size(size)
     return s, f"{unit}/s"
 
 
@@ -37,15 +39,15 @@
     Format datetime.timedelta into <days> <hours>:<minutes>:<seconds>.
     """
     minutes, seconds = divmod(delta.seconds, 60)
     hours, minutes = divmod(minutes, 60)
     return f"{delta.days:d} {hours:02d}:{minutes:02d}:{seconds:02d}"
 
 
-def get_torrent_arguments(rpc_version: int) -> List[str]:
+def get_torrent_arguments(rpc_version: int) -> list[str]:
     """
     Get torrent arguments for method in specified Transmission RPC version.
     """
     accessible = []
     for argument, info in constants.TORRENT_GET_ARGS.items():
         valid_version = True
         if rpc_version < info.added_version:
@@ -53,15 +55,15 @@
         if info.removed_version is not None and info.removed_version <= rpc_version:
             valid_version = False
         if valid_version:
             accessible.append(argument)
     return accessible
 
 
-def _try_read_torrent(torrent: Union[BinaryIO, str, bytes, pathlib.Path]) -> Optional[str]:  # pylint: disable=R0911
+def _try_read_torrent(torrent: BinaryIO | str | bytes | pathlib.Path) -> str | None:
     """
     if torrent should be encoded with base64, return a non-None value.
     """
     # torrent is a str, may be a url
     if isinstance(torrent, str):
         parsed_uri = urlparse(torrent)
         # torrent starts with file, read from local disk and encode it to base64 url.
```

### Comparing `transmission_rpc-7.0.6/PKG-INFO` & `transmission_rpc-7.0.7a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 7.0.6
+Version: 7.0.7a0
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
```

