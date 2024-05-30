# Comparing `tmp/olas_operate_middleware-0.1.0rc8.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc8.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc9.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc8.tar` & `olas_operate_middleware-0.1.0rc9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc8/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc8/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc8/operate/__init__.py
--rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc8/operate/account/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc8/operate/account/user.py
--rw-r--r--   0        0        0    19467 2024-04-19 10:21:51.397645 olas_operate_middleware-0.1.0rc8/operate/cli.py
--rw-r--r--   0        0        0     1189 2024-04-19 07:11:29.339849 olas_operate_middleware-0.1.0rc8/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc8/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc8/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc8/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc8/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc8/operate/keys.py
--rw-r--r--   0        0        0     3301 2024-04-17 09:26:07.366847 olas_operate_middleware-0.1.0rc8/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc8/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc8/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc8/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc8/operate/ledger/solana.py
--rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc8/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc8/operate/services/__init__.py
--rw-r--r--   0        0        0    18078 2024-04-19 09:58:14.889754 olas_operate_middleware-0.1.0rc8/operate/services/manage.py
--rw-r--r--   0        0        0    22899 2024-04-19 07:11:29.341358 olas_operate_middleware-0.1.0rc8/operate/services/protocol.py
--rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc8/operate/services/service.py
--rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc8/operate/types.py
--rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc8/operate/utils/__init__.py
--rw-r--r--   0        0        0     6333 2024-04-19 07:11:29.341902 olas_operate_middleware-0.1.0rc8/operate/utils/gnosis.py
--rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc8/operate/wallet/__init__.py
--rw-r--r--   0        0        0     8924 2024-04-19 07:11:29.342488 olas_operate_middleware-0.1.0rc8/operate/wallet/master.py
--rw-r--r--   0        0        0     1171 2024-04-19 10:29:44.300698 olas_operate_middleware-0.1.0rc8/pyproject.toml
--rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc8/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc9/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc9/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc9/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc9/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc9/operate/account/user.py
+-rw-r--r--   0        0        0    19467 2024-04-23 07:37:06.153607 olas_operate_middleware-0.1.0rc9/operate/cli.py
+-rw-r--r--   0        0        0     1189 2024-04-19 07:11:29.339849 olas_operate_middleware-0.1.0rc9/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc9/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc9/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc9/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc9/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc9/operate/keys.py
+-rw-r--r--   0        0        0     3301 2024-04-22 03:31:21.924276 olas_operate_middleware-0.1.0rc9/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc9/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc9/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc9/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc9/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc9/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc9/operate/services/__init__.py
+-rw-r--r--   0        0        0    18078 2024-04-23 07:37:06.154279 olas_operate_middleware-0.1.0rc9/operate/services/manage.py
+-rw-r--r--   0        0        0    22899 2024-04-19 07:11:29.341358 olas_operate_middleware-0.1.0rc9/operate/services/protocol.py
+-rw-r--r--   0        0        0    13695 2024-04-16 04:14:40.061038 olas_operate_middleware-0.1.0rc9/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc9/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc9/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6333 2024-04-19 07:11:29.341902 olas_operate_middleware-0.1.0rc9/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc9/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8924 2024-04-19 07:11:29.342488 olas_operate_middleware-0.1.0rc9/operate/wallet/master.py
+-rw-r--r--   0        0        0     1171 2024-04-23 11:38:52.703698 olas_operate_middleware-0.1.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     5668 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc9/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc8/LICENSE` & `olas_operate_middleware-0.1.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/README.md` & `olas_operate_middleware-0.1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/account/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/account/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/account/user.py` & `olas_operate_middleware-0.1.0rc9/operate/account/user.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/cli.py` & `olas_operate_middleware-0.1.0rc9/operate/cli.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/constants.py` & `olas_operate_middleware-0.1.0rc9/operate/constants.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc9/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc9/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/keys.py` & `olas_operate_middleware-0.1.0rc9/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc9/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc9/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc9/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc9/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/resource.py` & `olas_operate_middleware-0.1.0rc9/operate/resource.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc9/operate/services/manage.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc9/operate/services/protocol.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/services/service.py` & `olas_operate_middleware-0.1.0rc9/operate/services/service.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/types.py` & `olas_operate_middleware-0.1.0rc9/operate/types.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/utils/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/utils/gnosis.py` & `olas_operate_middleware-0.1.0rc9/operate/utils/gnosis.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/wallet/__init__.py` & `olas_operate_middleware-0.1.0rc9/operate/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/operate/wallet/master.py` & `olas_operate_middleware-0.1.0rc9/operate/wallet/master.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc8/pyproject.toml` & `olas_operate_middleware-0.1.0rc9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olas-operate-middleware"
-version = "0.1.0-rc8"
+version = "0.1.0-rc9"
 description = ""
 authors = ["David Vilela <dvilelaf@gmail.com>", "Viraj Patel <vptl185@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "operate" }
 ]
 include = [
```

### Comparing `olas_operate_middleware-0.1.0rc8/PKG-INFO` & `olas_operate_middleware-0.1.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

