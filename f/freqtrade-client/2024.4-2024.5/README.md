# Comparing `tmp/freqtrade_client-2024.4.tar.gz` & `tmp/freqtrade_client-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freqtrade_client-2024.4.tar", last modified: Tue Apr 30 12:41:58 2024, max compression
+gzip compressed data, was "freqtrade_client-2024.5.tar", last modified: Thu May 30 16:45:49 2024, max compression
```

## Comparing `freqtrade_client-2024.4.tar` & `freqtrade_client-2024.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/freqtrade_client/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/freqtrade_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/freqtrade_client/ft_client.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13616 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/freqtrade_client/ft_rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/freqtrade_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 12:41:58.000000 freqtrade_client-2024.4/freqtrade_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-30 12:41:47.000000 freqtrade_client-2024.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:41:58.578423 freqtrade_client-2024.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:45:49.355221 freqtrade_client-2024.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-30 16:45:49.355221 freqtrade_client-2024.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:45:49.351221 freqtrade_client-2024.5/freqtrade_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/freqtrade_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/freqtrade_client/ft_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13543 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/freqtrade_client/ft_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:45:49.355221 freqtrade_client-2024.5/freqtrade_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-30 16:45:49.000000 freqtrade_client-2024.5/freqtrade_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 16:45:49.000000 freqtrade_client-2024.5/freqtrade_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:45:49.000000 freqtrade_client-2024.5/freqtrade_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 16:45:49.000000 freqtrade_client-2024.5/freqtrade_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 16:45:49.000000 freqtrade_client-2024.5/freqtrade_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 16:45:49.000000 freqtrade_client-2024.5/freqtrade_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 16:45:37.000000 freqtrade_client-2024.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:45:49.355221 freqtrade_client-2024.5/setup.cfg
```

### Comparing `freqtrade_client-2024.4/LICENSE` & `freqtrade_client-2024.5/LICENSE`

 * *Files identical despite different names*

### Comparing `freqtrade_client-2024.4/PKG-INFO` & `freqtrade_client-2024.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freqtrade-client
-Version: 2024.4
+Version: 2024.5
 Summary: Freqtrade - Client scripts
 Author: Freqtrade Team
 Author-email: Freqtrade Team <freqtrade@protonmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/freqtrade/freqtrade
 Project-URL: Documentation, https://freqtrade.io
 Project-URL: Bug Tracker, https://github.com/freqtrade/freqtrade/issues
```

### Comparing `freqtrade_client-2024.4/freqtrade_client/__init__.py` & `freqtrade_client-2024.5/freqtrade_client/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 from freqtrade_client.ft_rest_client import FtRestClient
 
 
-__version__ = '2024.4'
+__version__ = "2024.5"
 
-if 'dev' in __version__:
+if "dev" in __version__:
     from pathlib import Path
+
     try:
         import subprocess
+
         freqtrade_basedir = Path(__file__).parent
 
-        __version__ = __version__ + '-' + subprocess.check_output(
-            ['git', 'log', '--format="%h"', '-n 1'],
-            stderr=subprocess.DEVNULL, cwd=freqtrade_basedir).decode("utf-8").rstrip().strip('"')
+        __version__ = (
+            __version__
+            + "-"
+            + subprocess.check_output(
+                ["git", "log", '--format="%h"', "-n 1"],
+                stderr=subprocess.DEVNULL,
+                cwd=freqtrade_basedir,
+            )
+            .decode("utf-8")
+            .rstrip()
+            .strip('"')
+        )
 
     except Exception:  # pragma: no cover
         # git not available, ignore
         try:
             # Try Fallback to freqtrade_commit file (created by CI while building docker image)
-            versionfile = Path('./freqtrade_commit')
+            versionfile = Path("./freqtrade_commit")
             if versionfile.is_file():
                 __version__ = f"docker-{__version__}-{versionfile.read_text()[:8]}"
         except Exception:
             pass
 
-__all__ = ['FtRestClient']
+__all__ = ["FtRestClient"]
```

### Comparing `freqtrade_client-2024.4/freqtrade_client/ft_client.py` & `freqtrade_client-2024.5/freqtrade_client/ft_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,98 +4,102 @@
 import logging
 import re
 import sys
 from pathlib import Path
 from typing import Any, Dict
 
 import rapidjson
+
 from freqtrade_client import __version__
 from freqtrade_client.ft_rest_client import FtRestClient
 
 
 logging.basicConfig(
     level=logging.INFO,
-    format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
+    format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
 )
 logger = logging.getLogger("ft_rest_client")
 
 
 def add_arguments(args: Any = None):
     parser = argparse.ArgumentParser(
-            prog="freqtrade-client",
-            description="Client for the freqtrade REST API",
+        prog="freqtrade-client",
+        description="Client for the freqtrade REST API",
+    )
+    parser.add_argument(
+        "command", help="Positional argument defining the command to execute.", nargs="?"
+    )
+    parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {__version__}")
+    parser.add_argument(
+        "--show",
+        help="Show possible methods with this client",
+        dest="show",
+        action="store_true",
+        default=False,
+    )
+
+    parser.add_argument(
+        "-c",
+        "--config",
+        help="Specify configuration file (default: %(default)s). ",
+        dest="config",
+        type=str,
+        metavar="PATH",
+        default="config.json",
+    )
+
+    parser.add_argument(
+        "command_arguments",
+        help="Positional arguments for the parameters for [command]",
+        nargs="*",
+        default=[],
     )
-    parser.add_argument("command",
-                        help="Positional argument defining the command to execute.",
-                        nargs="?"
-                        )
-    parser.add_argument('-V', '--version', action='version', version=f'%(prog)s {__version__}')
-    parser.add_argument('--show',
-                        help='Show possible methods with this client',
-                        dest='show',
-                        action='store_true',
-                        default=False
-                        )
-
-    parser.add_argument('-c', '--config',
-                        help='Specify configuration file (default: %(default)s). ',
-                        dest='config',
-                        type=str,
-                        metavar='PATH',
-                        default='config.json'
-                        )
-
-    parser.add_argument("command_arguments",
-                        help="Positional arguments for the parameters for [command]",
-                        nargs="*",
-                        default=[]
-                        )
 
     pargs = parser.parse_args(args)
     return vars(pargs)
 
 
 def load_config(configfile):
     file = Path(configfile)
     if file.is_file():
         with file.open("r") as f:
-            config = rapidjson.load(f, parse_mode=rapidjson.PM_COMMENTS |
-                                    rapidjson.PM_TRAILING_COMMAS)
+            config = rapidjson.load(
+                f, parse_mode=rapidjson.PM_COMMENTS | rapidjson.PM_TRAILING_COMMAS
+            )
         return config
     else:
         logger.warning(f"Could not load config file {file}.")
         sys.exit(1)
 
 
 def print_commands():
     # Print dynamic help for the different commands using the commands doc-strings
     client = FtRestClient(None)
     print("Possible commands:\n")
     for x, _ in inspect.getmembers(client):
-        if not x.startswith('_'):
-            doc = re.sub(':return:.*', '', getattr(client, x).__doc__, flags=re.MULTILINE).rstrip()
+        if not x.startswith("_"):
+            doc = re.sub(":return:.*", "", getattr(client, x).__doc__, flags=re.MULTILINE).rstrip()
             print(f"{x}\n\t{doc}\n")
 
 
 def main_exec(args: Dict[str, Any]):
-
     if args.get("show"):
         print_commands()
         sys.exit()
 
-    config = load_config(args['config'])
-    url = config.get('api_server', {}).get('listen_ip_address', '127.0.0.1')
-    port = config.get('api_server', {}).get('listen_port', '8080')
-    username = config.get('api_server', {}).get('username')
-    password = config.get('api_server', {}).get('password')
+    config = load_config(args["config"])
+    url = config.get("api_server", {}).get("listen_ip_address", "127.0.0.1")
+    port = config.get("api_server", {}).get("listen_port", "8080")
+    username = config.get("api_server", {}).get("username")
+    password = config.get("api_server", {}).get("password")
 
     server_url = f"http://{url}:{port}"
     client = FtRestClient(server_url, username, password)
 
-    m = [x for x, y in inspect.getmembers(client) if not x.startswith('_')]
+    m = [x for x, y in inspect.getmembers(client) if not x.startswith("_")]
     command = args["command"]
     if command not in m:
         logger.error(f"Command {command} not defined")
         print_commands()
         return
 
     print(json.dumps(getattr(client, command)(*args["command_arguments"])))
```

### Comparing `freqtrade_client-2024.4/freqtrade_client/ft_rest_client.py` & `freqtrade_client-2024.5/freqtrade_client/ft_rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,39 +17,34 @@
 logger = logging.getLogger("ft_rest_client")
 
 ParamsT = Optional[Dict[str, Any]]
 PostDataT = Optional[Union[Dict[str, Any], List[Dict[str, Any]]]]
 
 
 class FtRestClient:
-
-    def __init__(self, serverurl, username=None, password=None, *,
-                 pool_connections=10, pool_maxsize=10):
-
+    def __init__(
+        self, serverurl, username=None, password=None, *, pool_connections=10, pool_maxsize=10
+    ):
         self._serverurl = serverurl
         self._session = requests.Session()
 
         # allow configuration of pool
         adapter = requests.adapters.HTTPAdapter(
-            pool_connections=pool_connections,
-            pool_maxsize=pool_maxsize
+            pool_connections=pool_connections, pool_maxsize=pool_maxsize
         )
-        self._session.mount('http://', adapter)
+        self._session.mount("http://", adapter)
 
         self._session.auth = (username, password)
 
     def _call(self, method, apipath, params: Optional[dict] = None, data=None, files=None):
-
-        if str(method).upper() not in ('GET', 'POST', 'PUT', 'DELETE'):
-            raise ValueError(f'invalid method <{method}>')
+        if str(method).upper() not in ("GET", "POST", "PUT", "DELETE"):
+            raise ValueError(f"invalid method <{method}>")
         basepath = f"{self._serverurl}/api/v1/{apipath}"
 
-        hd = {"Accept": "application/json",
-              "Content-Type": "application/json"
-              }
+        hd = {"Accept": "application/json", "Content-Type": "application/json"}
 
         # Split url
         schema, netloc, path, par, query, fragment = urlparse(basepath)
         # URLEncode query string
         query = urlencode(params) if params else ""
         # recombine url
         url = urlunparse((schema, netloc, path, par, query, fragment))
@@ -147,31 +142,24 @@
         """Delete (disable) lock from the database.
 
         :param lock_id: ID for the lock to delete
         :return: json object
         """
         return self._delete(f"locks/{lock_id}")
 
-    def lock_add(self, pair: str, until: str, side: str = '*', reason: str = ''):
+    def lock_add(self, pair: str, until: str, side: str = "*", reason: str = ""):
         """Lock pair
 
         :param pair: Pair to lock
         :param until: Lock until this date (format "2024-03-30 16:00:00Z")
         :param side: Side to lock (long, short, *)
         :param reason: Reason for the lock
         :return: json object
         """
-        data = [
-            {
-                "pair": pair,
-                "until": until,
-                "side": side,
-                "reason": reason
-            }
-        ]
+        data = [{"pair": pair, "until": until, "side": side, "reason": reason}]
         return self._post("locks", data=data)
 
     def daily(self, days=None):
         """Return the profits for each day, and amount of trades.
 
         :return: json object
         """
@@ -230,25 +218,25 @@
         """Return the version of the bot.
 
         :return: json object containing the version
         """
         return self._get("version")
 
     def show_config(self):
-        """ Returns part of the configuration, relevant for trading operations.
+        """Returns part of the configuration, relevant for trading operations.
         :return: json object containing the version
         """
         return self._get("show_config")
 
     def ping(self):
         """simple ping"""
         configstatus = self.show_config()
         if not configstatus:
             return {"status": "not_running"}
-        elif configstatus['state'] == "running":
+        elif configstatus["state"] == "running":
             return {"status": "pong"}
         else:
             return {"status": "not_running"}
 
     def logs(self, limit=None):
         """Show latest logs.
 
@@ -262,17 +250,17 @@
 
         :param limit: Limits trades to the X last trades. Max 500 trades.
         :param offset: Offset by this amount of trades.
         :return: json object
         """
         params = {}
         if limit:
-            params['limit'] = limit
+            params["limit"] = limit
         if offset:
-            params['offset'] = offset
+            params["offset"] = offset
         return self._get("trades", params)
 
     def trade(self, trade_id):
         """Return specific trade
 
         :param trade_id: Specify which trade to get.
         :return: json object
@@ -317,48 +305,50 @@
     def forcebuy(self, pair, price=None):
         """Buy an asset.
 
         :param pair: Pair to buy (ETH/BTC)
         :param price: Optional - price to buy
         :return: json object of the trade
         """
-        data = {"pair": pair,
-                "price": price
-                }
+        data = {"pair": pair, "price": price}
         return self._post("forcebuy", data=data)
 
     def forceenter(self, pair, side, price=None):
         """Force entering a trade
 
         :param pair: Pair to buy (ETH/BTC)
         :param side: 'long' or 'short'
         :param price: Optional - price to buy
         :return: json object of the trade
         """
-        data = {"pair": pair,
-                "side": side,
-                }
+        data = {
+            "pair": pair,
+            "side": side,
+        }
         if price:
-            data['price'] = price
+            data["price"] = price
         return self._post("forceenter", data=data)
 
     def forceexit(self, tradeid, ordertype=None, amount=None):
         """Force-exit a trade.
 
         :param tradeid: Id of the trade (can be received via status command)
         :param ordertype: Order type to use (must be market or limit)
         :param amount: Amount to sell. Full sell if not given
         :return: json object
         """
 
-        return self._post("forceexit", data={
-            "tradeid": tradeid,
-            "ordertype": ordertype,
-            "amount": amount,
-            })
+        return self._post(
+            "forceexit",
+            data={
+                "tradeid": tradeid,
+                "ordertype": ordertype,
+                "amount": amount,
+            },
+        )
 
     def strategies(self):
         """Lists available strategies
 
         :return: json object
         """
         return self._get("strategies")
@@ -388,18 +378,21 @@
     def available_pairs(self, timeframe=None, stake_currency=None):
         """Return available pair (backtest data) based on timeframe / stake_currency selection
 
         :param timeframe: Only pairs with this timeframe available.
         :param stake_currency: Only pairs that include this timeframe
         :return: json object
         """
-        return self._get("available_pairs", params={
-            "stake_currency": stake_currency if timeframe else '',
-            "timeframe": timeframe if timeframe else '',
-        })
+        return self._get(
+            "available_pairs",
+            params={
+                "stake_currency": stake_currency if timeframe else "",
+                "timeframe": timeframe if timeframe else "",
+            },
+        )
 
     def pair_candles(self, pair, timeframe, limit=None, columns=None):
         """Return live dataframe for <pair><timeframe>.
 
         :param pair: Pair to get data for
         :param timeframe: Only pairs with this timeframe available.
         :param limit: Limit result to the last n candles.
@@ -407,42 +400,42 @@
         :return: json object
         """
         params = {
             "pair": pair,
             "timeframe": timeframe,
         }
         if limit:
-            params['limit'] = limit
+            params["limit"] = limit
 
         if columns is not None:
-            params['columns'] = columns
-            return self._post(
-                "pair_candles",
-                data=params
-            )
+            params["columns"] = columns
+            return self._post("pair_candles", data=params)
 
         return self._get("pair_candles", params=params)
 
     def pair_history(self, pair, timeframe, strategy, timerange=None, freqaimodel=None):
         """Return historic, analyzed dataframe
 
         :param pair: Pair to get data for
         :param timeframe: Only pairs with this timeframe available.
         :param strategy: Strategy to analyze and get values for
         :param freqaimodel: FreqAI model to use for analysis
         :param timerange: Timerange to get data for (same format than --timerange endpoints)
         :return: json object
         """
-        return self._get("pair_history", params={
-            "pair": pair,
-            "timeframe": timeframe,
-            "strategy": strategy,
-            "freqaimodel": freqaimodel,
-            "timerange": timerange if timerange else '',
-        })
+        return self._get(
+            "pair_history",
+            params={
+                "pair": pair,
+                "timeframe": timeframe,
+                "strategy": strategy,
+                "freqaimodel": freqaimodel,
+                "timerange": timerange if timerange else "",
+            },
+        )
 
     def sysinfo(self):
         """Provides system information (CPU, RAM usage)
 
         :return: json object
         """
         return self._get("sysinfo")
```

### Comparing `freqtrade_client-2024.4/freqtrade_client.egg-info/PKG-INFO` & `freqtrade_client-2024.5/freqtrade_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freqtrade-client
-Version: 2024.4
+Version: 2024.5
 Summary: Freqtrade - Client scripts
 Author: Freqtrade Team
 Author-email: Freqtrade Team <freqtrade@protonmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/freqtrade/freqtrade
 Project-URL: Documentation, https://freqtrade.io
 Project-URL: Bug Tracker, https://github.com/freqtrade/freqtrade/issues
```

### Comparing `freqtrade_client-2024.4/pyproject.toml` & `freqtrade_client-2024.5/pyproject.toml`

 * *Files identical despite different names*

