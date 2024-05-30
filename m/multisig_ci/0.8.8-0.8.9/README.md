# Comparing `tmp/multisig_ci-0.8.8.tar.gz` & `tmp/multisig_ci-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.8.8.tar", max compression
+gzip compressed data, was "multisig_ci-0.8.9.tar", max compression
```

## Comparing `multisig_ci-0.8.8.tar` & `multisig_ci-0.8.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/LICENSE
--rw-r--r--   0        0        0        0 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/__main__.py
--rw-r--r--   0        0        0     7125 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2633 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      887 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/safes.py
--rw-r--r--   0        0        0     1579 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      505 2023-12-31 00:43:34.501473 multisig_ci-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 multisig_ci-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     7123 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2631 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      887 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1579 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      505 2023-12-31 00:55:01.767085 multisig_ci-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 multisig_ci-0.8.9/PKG-INFO
```

### Comparing `multisig_ci-0.8.8/LICENSE` & `multisig_ci-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/multisig_ci/__main__.py` & `multisig_ci-0.8.9/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/multisig_ci/ci_override.py` & `multisig_ci-0.8.9/multisig_ci/ci_override.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         traces_sample_rate=1.0,
         # Set profiles_sample_rate to 1.0 to profile 100%
         # of sampled transactions.
         # We recommend adjusting this value in production.
         profiles_sample_rate=1.0,
     )
     print("Sentry initialized!")
-except ImportError:
+except Exception:
     pass
 
 def mine_override(timestamp: Optional[int] = None) -> None:
     if timestamp:
         anvil._request("evm_setNextBlockTimestamp", [timestamp])
     anvil._request("evm_mine", [])
```

### Comparing `multisig_ci-0.8.8/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.8.9/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/multisig_ci/run_brownie.py` & `multisig_ci-0.8.9/multisig_ci/run_brownie.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         traces_sample_rate=1.0,
         # Set profiles_sample_rate to 1.0 to profile 100%
         # of sampled transactions.
         # We recommend adjusting this value in production.
         profiles_sample_rate=1.0,
     )
     print("Sentry initialized!")
-except ImportError:
+except Exception:
     pass
 
 @retry(stop=stop_after_attempt(5))
 def run_brownie(args):
     global current_try_count
 
     # Kill processes to make sure we start clean
```

### Comparing `multisig_ci-0.8.8/multisig_ci/safes.py` & `multisig_ci-0.8.9/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/multisig_ci/sign.py` & `multisig_ci-0.8.9/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/multisig_ci/telegram.py` & `multisig_ci-0.8.9/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/multisig_ci/test_telegram.sh` & `multisig_ci-0.8.9/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.8.8/PKG-INFO` & `multisig_ci-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisig_ci
-Version: 0.8.8
+Version: 0.8.9
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

