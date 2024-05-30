# Comparing `tmp/pass_operator-0.4.3.tar.gz` & `tmp/pass_operator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass_operator-0.4.3.tar", max compression
+gzip compressed data, was "pass_operator-0.4.4.tar", max compression
```

## Comparing `pass_operator-0.4.3.tar` & `pass_operator-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35140 2024-05-29 15:42:34.395919 pass_operator-0.4.3/LICENSE
--rw-r--r--   0        0        0     3338 2024-05-29 15:42:34.395919 pass_operator-0.4.3/README.md
--rw-r--r--   0        0        0     1606 2024-05-29 15:42:49.516004 pass_operator-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1562 2024-05-29 15:42:34.399919 pass_operator-0.4.3/src/passoperator/__init__.py
--rw-r--r--   0        0        0    15025 2024-05-29 15:42:34.399919 pass_operator-0.4.3/src/passoperator/daemon.py
--rw-r--r--   0        0        0     2017 2024-05-29 15:42:34.399919 pass_operator-0.4.3/src/passoperator/git.py
--rw-r--r--   0        0        0     1218 2024-05-29 15:42:34.399919 pass_operator-0.4.3/src/passoperator/gpg.py
--rw-r--r--   0        0        0     8500 2024-05-29 15:42:34.399919 pass_operator-0.4.3/src/passoperator/secret.py
--rw-r--r--   0        0        0     1313 2024-05-29 15:42:34.399919 pass_operator-0.4.3/src/passoperator/utils.py
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 pass_operator-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35140 2024-05-30 19:29:50.572975 pass_operator-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3727 2024-05-30 19:29:50.572975 pass_operator-0.4.4/README.md
+-rw-r--r--   0        0        0     1612 2024-05-30 19:30:05.693122 pass_operator-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1670 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/__init__.py
+-rw-r--r--   0        0        0    17134 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/daemon.py
+-rw-r--r--   0        0        0     2017 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/git.py
+-rw-r--r--   0        0        0     1213 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/gpg.py
+-rw-r--r--   0        0        0     9217 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/secret.py
+-rw-r--r--   0        0        0     1313 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/utils.py
+-rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 pass_operator-0.4.4/PKG-INFO
```

### Comparing `pass_operator-0.4.3/LICENSE` & `pass_operator-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.3/README.md` & `pass_operator-0.4.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # `pass` secrets operator
 
+![GitHub Release](https://img.shields.io/github/v/release/premiscale/pass-operator)
+![PyPI - License](https://img.shields.io/pypi/l/pass-operator)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pass-operator)
+![Docker Pulls](https://img.shields.io/docker/pulls/premiscale/pass-operator)
+![CircleCI](https://img.shields.io/circleci/build/github/premiscale/pass-operator)
+
+
 A Kubernetes operator to sync and decrypt secrets from a password store ([pass](https://www.passwordstore.org/)) Git repository. This operator is proposed as a proof-of-concept and shouldn't be used in any production capacity.
 
 While this approach to secrets management on Kubernetes is more technically challenging, the advantage is that we don't have to rely on a 3rd party SaaS platform, such as Vault or Doppler, to hold our secrets (the obvious benefits these platforms do provide, however, are better user and access management). We may also use this operator in an airgapped environment with a self-hosted git repository.
 
 <!--
 I also acknowledge that this approach swims against the DevSecOps tide in that it requires you to store your secrets (albeit encrypted)
 in Git, a practice that is often discouraged and typically forbidden at most organizations.
```

### Comparing `pass_operator-0.4.3/pyproject.toml` & `pass_operator-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pass-operator"
-version = "v0.4.3"
-description = "A kubernetes operator that syncs and decrypts secrets from pass git repositories"
+version = "v0.4.4"
+description = "A Kubernetes operator that syncs and decrypts secrets from pass store git repositories"
 authors = ["Emma Doyle <emma@premiscale.com>"]
 maintainers = ["Emma Doyle <emma@premiscale.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
   { include = "passoperator", from = "src" }
 ]
```

### Comparing `pass_operator-0.4.3/src/passoperator/__init__.py` & `pass_operator-0.4.4/src/passoperator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,20 +32,22 @@
     # Environment variables to configure pass.
     'PASS_BINARY':            os.getenv('PASS_BINARY', '/usr/bin/pass'),
     'PASS_DIRECTORY':         str(Path(f'~/.password-store/{os.getenv("PASS_DIRECTORY", "")}').expanduser()),
     'PASS_GPG_PASSPHRASE':    os.getenv('PASS_GPG_PASSPHRASE', ''),
     'PASS_GPG_KEY':           os.getenv('PASS_GPG_KEY', ''),
     'PASS_GPG_KEY_ID':        os.getenv('PASS_GPG_KEY_ID', ''),
     'PASS_GIT_URL':           os.getenv('PASS_GIT_URL', ''),
-    'PASS_GIT_BRANCH':        os.getenv('PASS_GIT_BRANCH', 'main')
+    'PASS_GIT_BRANCH':        os.getenv('PASS_GIT_BRANCH', 'main'),
+    'PASS_DECRYPT_THREADS':   os.getenv('PASS_DECRYPT_THREADS', '4'),
 }
 
 
 # Environment type validation.
 try:
     float(env['OPERATOR_INTERVAL'])
     float(env['OPERATOR_INITIAL_DELAY'])
     int(env['OPERATOR_PRIORITY'])
     IPv4Address(env['OPERATOR_POD_IP'])
+    int(env['PASS_DECRYPT_THREADS'])
 except (ValueError, AddressValueError) as e:
     log.error(e)
     sys.exit(1)
```

### Comparing `pass_operator-0.4.3/src/passoperator/daemon.py` & `pass_operator-0.4.4/src/passoperator/daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A kubernetes operator that syncs and decrypts secrets from Linux password store (https://www.passwordstore.org/) git repositories.
 """
 
 
-from typing import Any
+from typing import Any, List, Tuple
 from pathlib import Path
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from importlib import metadata
 from kubernetes import client, config
 from http import HTTPStatus
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
@@ -23,14 +23,63 @@
 import kopf
 
 
 __version__ = metadata.version('pass-operator')
 
 log = logging.getLogger(__name__)
 
+__in_progress_queue: List[Tuple[Any, Any]] = []
+
+
+def _passsecret_block(body: kopf.Body) -> None:
+    """
+    Block handlers' progress on a PassSecret until it's safe to modify the managed secret.
+    Decryption takes time, so we want to be sure to queue up any changes.
+
+    Args:
+        body [kopf.Body]: raw body of the PassSecret.
+    """
+    __in_progress_queue.append(
+        (
+            body['metadata']['name'],
+            body['metadata']['namespace']
+        )
+    )
+
+
+def _is_passsecret_blocked(body: kopf.Body) -> bool:
+    """
+    Check if a PassSecret is blocked from modification.
+
+    Args:
+        body [kopf.Body]: raw body of the PassSecret.
+
+    Returns:
+        bool: True if the PassSecret is blocked, else False.
+    """
+    return (
+        body['metadata']['name'],
+        body['metadata']['namespace']
+    ) in __in_progress_queue
+
+
+def _lift_passsecret_block(body: kopf.Body) -> None:
+    """
+    Unblock handlers' progress to modify the managed secret.
+
+    Args:
+        body [kopf.Body]: raw body of the PassSecret.
+    """
+    __in_progress_queue.remove(
+        (
+            body['metadata']['name'],
+            body['metadata']['namespace']
+        )
+    )
+
 
 @kopf.on.startup()
 def start(settings: kopf.OperatorSettings, **_: Any) -> None:
     """
     Set up operator runtime.
     """
     log.info(f'Starting operator version {__version__}')
@@ -39,43 +88,47 @@
 
 
 @kopf.timer(
     # Target PassSecret.secrets.premiscale.com/v1alpha1
     'secrets.premiscale.com', 'v1alpha1', 'passsecret',
     # Interval to check every instance of a PassSecret.
     interval=float(env['OPERATOR_INTERVAL']),
-    # Initial delay in seconds before reviewing all managed PassSecrets.
+    # Initial delay in seconds before reviewing managed PassSecrets.
     initial_delay=float(env['OPERATOR_INITIAL_DELAY']),
     # Don't delay if the prior reconciliation hasn't completed.
     sharp=True)
 def reconciliation(body: kopf.Body, **_: Any) -> None:
     """
     Reconcile state of a managed secret against the pass store. Update secrets' data if a mismatch
     is found. Kopf timers are triggered on an object-by-object basis, so this method will
     automatically revisit every PassSecret, iff it resides in the same namespace as the operator.
 
     Args:
         body [kopf.Body]: raw body of the PassSecret.
     """
 
+    # Before we parse and decrypt anything, which is more expensive, check if this PassSecret is already in progress.
+    if _is_passsecret_blocked(body):
+        log.info(f'PassSecret "{body["metadata"]["name"]}" is still in progress. Skipping.')
+        return None
+
     # Ensure the GPG key ID in ~/.password-store/${PASS_DIRECTORY}/.gpg-id did not change with the git update.
     check_gpg_id(
         path=f'{env["PASS_DIRECTORY"]}/.gpg-id'
     )
 
+    v1 = client.CoreV1Api()
+
     # Create a new PassSecret object with an up-to-date managedSecret decrypted value from the pass store.
     passSecretObj = PassSecret.from_kopf(body)
 
     log.info(
         f'Reconciling PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}" against password store.'
     )
 
-    v1 = client.CoreV1Api()
-
-
     try:
         secret = v1.read_namespaced_secret(
             name=passSecretObj.spec.managedSecret.metadata.name,
             namespace=passSecretObj.spec.managedSecret.metadata.namespace
         )
 
         log.debug(secret)
@@ -109,14 +162,15 @@
                 body=client.V1Secret(
                     **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
         else:
             raise kopf.PermanentError(e)
 
+
 # @kopf.on.cleanup()
 # def cleanup(**kwargs) -> None:
 #     pass
 
 # @kopf.on.resume()
 # def resume(**kwargs) -> None:
 #     pass
@@ -148,52 +202,57 @@
         else:
             return None
     except client.ApiException as e:
         raise kopf.PermanentError(e)
 
 
 @kopf.on.update('secrets.premiscale.com', 'v1alpha1', 'passsecret')
-def update(old: kopf.BodyEssence | Any, new: kopf.BodyEssence | Any, meta: kopf.Meta, **_: Any) -> None:
+def update(old: kopf.BodyEssence | Any, new: kopf.BodyEssence | Any, meta: kopf.Meta, body: kopf.Body, **_: Any) -> None:
     """
     An update was received on the PassSecret object, so attempt to update the corresponding Secret.
 
     This method is pretty much identical to 'create'-type events.
 
     Args:
         body [kopf.Body]: raw body of the PassSecret.
+        meta [kopf.Meta]: metadata of the PassSecret.
         old [kopf.BodyEssence]: old body of the PassSecret.
         new [kopf.BodyEssence]: new body of the PassSecret.
     """
     metadata = {
         'metadata': {
             'name': meta['name'],
             'namespace': meta['namespace']
         }
     }
 
+    _passsecret_block(body)
+
     # Parse the old PassSecret manifest.
     try:
         oldPassSecret = PassSecret.from_kopf(
             {
                 **metadata,
                 **old
             }
         )
     except (ValueError, KeyError) as e:
+        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     # Parse the new PassSecret manifest.
     try:
         newPassSecret = PassSecret.from_kopf(
             {
                 **metadata,
                 **new
             }
         )
     except (ValueError, KeyError) as e:
+        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     v1 = client.CoreV1Api()
 
     # Handle typically immutable field changes separately from the rest of the manifest on Secrets.
     try:
         if newPassSecret.spec.managedSecret.metadata.namespace != oldPassSecret.spec.managedSecret.metadata.namespace or newPassSecret.spec.managedSecret.metadata.name != oldPassSecret.spec.managedSecret.metadata.name:
@@ -220,60 +279,74 @@
             )
 
         log.info(
             f'Successfully updated PassSecret "{newPassSecret.metadata.name}" managed Secret "{newPassSecret.spec.managedSecret.metadata.name}".'
         )
     except client.ApiException as e:
         raise kopf.PermanentError(e)
+    finally:
+        _lift_passsecret_block(body)
 
 
 @kopf.on.create('secrets.premiscale.com', 'v1alpha1', 'passsecret')
 def create(body: kopf.Body, **_: Any) -> None:
     """
     Create a new Secret with the spec of the newly-created PassSecret.
 
     Args:
         body [kopf.Body]: raw body of the created PassSecret.
     """
     try:
+        # Indicate to the reconciliation loop that this PassSecret is in progress.
+        _passsecret_block(body)
+
         passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
+        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     log.info(f'PassSecret "{passSecretObj.metadata.name}" created')
 
     v1 = client.CoreV1Api()
 
     try:
         v1.create_namespaced_secret(
             namespace=passSecretObj.spec.managedSecret.metadata.namespace,
             body=client.V1Secret(
                 **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
             )
         )
+
         log.info(
             f'Created PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}"'
         )
     except client.ApiException as e:
         if e.status == HTTPStatus.CONFLICT:
             raise kopf.TemporaryError(f'Duplicate PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}". Skipping.')
+
         raise kopf.PermanentError(e)
+    finally:
+        _lift_passsecret_block(body)
 
 
 @kopf.on.delete('secrets.premiscale.com', 'v1alpha1', 'passsecret')
 def delete(body: kopf.Body, **_: Any) -> None:
     """
     Remove a managed secret, as the managing PassSecret has been deleted.
 
     Args:
         body [kopf.Body]: raw body of the deleted PassSecret.
     """
     try:
+        # Indicate to the reconciliation loop that this PassSecret is in progress.
+        _passsecret_block(body)
+
         passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
+        _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     log.info(f'PassSecret "{passSecretObj.metadata.name}" deleted')
 
     v1 = client.CoreV1Api()
 
     try:
@@ -282,14 +355,16 @@
             namespace=passSecretObj.spec.managedSecret.metadata.namespace
         )
         log.info(f'Deleted PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}"')
     except client.ApiException as e:
         if e.status == HTTPStatus.NOT_FOUND:
             log.warning(f'PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" was not found. Skipping.')
         raise kopf.PermanentError(e)
+    finally:
+        _lift_passsecret_block(body)
 
 
 def check_gpg_id(path: Path | str, remove: bool =False) -> None:
     """
     Ensure the gpg ID exists (leftover from 'pass init' in the entrypoint, or a git clone) and its contents match PASS_GPG_KEY_ID.
 
     Args:
```

### Comparing `pass_operator-0.4.3/src/passoperator/git.py` & `pass_operator-0.4.4/src/passoperator/git.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.3/src/passoperator/gpg.py` & `pass_operator-0.4.4/src/passoperator/gpg.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     gpg = GPG(
         gnupghome=home
     )
 
     try:
         # https://gnupg.readthedocs.io/en/latest/#decryption
         decrypted_file = gpg.decrypt_file(
-            f'{str(path)}.gpg',
+            f'{path}.gpg',
             always_trust=True,
             passphrase=passphrase
         )
 
         return str(decrypted_file).rstrip()
     except (IOError, PermissionError) as e:
         log.error(e)
```

### Comparing `pass_operator-0.4.3/src/passoperator/secret.py` & `pass_operator-0.4.4/src/passoperator/secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from __future__ import annotations
 from typing import Dict, Final, List
 from pathlib import Path
 from attrs import define, asdict as to_dict
 from cattrs import structure as from_dict
 from humps import camelize
 from datetime import datetime
+from concurrent.futures import ThreadPoolExecutor
 
 from passoperator.gpg import decrypt
 from passoperator.utils import b64Dec, b64Enc
 from passoperator import env
 
 import kopf
 import logging
@@ -117,19 +118,26 @@
         """
         Output this secret to a dictionary with keys that match the arguments of kubernetes.client.V1Secret, for convenience.
 
         Args:
             finalizers (bool): if True, include the finalizers field in the output.
         """
         d = dict(self.to_dict(export=True))
-        d.pop('data')
+
+        # Refine the data a bit so it corresponds to the k8s.client.V1Secret object.
+        if 'data' in d and not d['data']:
+            d.pop('data')
+
         d.pop('apiVersion')
+
         if not finalizers:
             d.pop('finalizers')
+
         d['string_data'] = self.stringData
+
         return d
 
     def __eq__(self, __value: object) -> bool:
         """
         Compare two ManagedSecrets.
 
         Returns:
@@ -189,27 +197,37 @@
     @staticmethod
     def decrypt(ms: ManagedSecret, encryptedData: Dict[str, str]) -> ManagedSecret:
         """
         Decrypt the contents of this PassSecret's paths before returning the spec object.
         """
         stringData = {}
 
-        for secretKey in encryptedData:
-            secretPath = encryptedData[secretKey]
+        with ThreadPoolExecutor(max_workers=int(env['PASS_DECRYPT_THREADS'])) as executor:
+            threads: Dict = {}
+
+            # Decrypt each secret in a separate thread and store the result in a dictionary.
+            for secretKey in encryptedData:
+                secretPath = encryptedData[secretKey]
+
+                # Because we're only decrypting, this operation should be threadsafe.
+                threads[secretKey] = executor.submit(
+                    decrypt,
+                    Path(f'{env["PASS_DIRECTORY"]}/{secretPath}'),
+                    passphrase=env['PASS_GPG_PASSPHRASE']
+                )
+
+            for secretKey in threads:
+                thread = threads[secretKey]
+                decryptedSecret = thread.result()
 
-            decryptedSecret = decrypt(
-                Path(f'{env["PASS_DIRECTORY"]}/{secretPath}'),
-                passphrase=env['PASS_GPG_PASSPHRASE']
-            )
-
-            if decryptedSecret:
-                stringData[secretKey] = decryptedSecret
-            else:
-                log.error(f'Failed to decrypt secret at path: {secretPath}')
-                stringData[secretKey] = ''
+                if decryptedSecret is not None:
+                    stringData[secretKey] = decryptedSecret
+                else:
+                    log.error(f'Failed to decrypt secret at path: {secretPath}')
+                    stringData[secretKey] = ''
 
         return ManagedSecret(
             metadata=ms.metadata,
             stringData=stringData,
             immutable=ms.immutable,
             type=ms.type
         )
```

### Comparing `pass_operator-0.4.3/src/passoperator/utils.py` & `pass_operator-0.4.4/src/passoperator/utils.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.3/PKG-INFO` & `pass_operator-0.4.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pass-operator
-Version: 0.4.3
-Summary: A kubernetes operator that syncs and decrypts secrets from pass git repositories
+Version: 0.4.4
+Summary: A Kubernetes operator that syncs and decrypts secrets from pass store git repositories
 License: GPL-3.0-or-later
 Keywords: python,kubernetes,secrets,operator,pass
 Author: Emma Doyle
 Author-email: emma@premiscale.com
 Maintainer: Emma Doyle
 Maintainer-email: emma@premiscale.com
 Requires-Python: >=3.10,<4.0
@@ -21,14 +21,21 @@
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: pyhumps (>=3.8.0,<4.0.0)
 Requires-Dist: python-gnupg (>=0.5.2,<0.6.0)
 Description-Content-Type: text/markdown
 
 # `pass` secrets operator
 
+![GitHub Release](https://img.shields.io/github/v/release/premiscale/pass-operator)
+![PyPI - License](https://img.shields.io/pypi/l/pass-operator)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pass-operator)
+![Docker Pulls](https://img.shields.io/docker/pulls/premiscale/pass-operator)
+![CircleCI](https://img.shields.io/circleci/build/github/premiscale/pass-operator)
+
+
 A Kubernetes operator to sync and decrypt secrets from a password store ([pass](https://www.passwordstore.org/)) Git repository. This operator is proposed as a proof-of-concept and shouldn't be used in any production capacity.
 
 While this approach to secrets management on Kubernetes is more technically challenging, the advantage is that we don't have to rely on a 3rd party SaaS platform, such as Vault or Doppler, to hold our secrets (the obvious benefits these platforms do provide, however, are better user and access management). We may also use this operator in an airgapped environment with a self-hosted git repository.
 
 <!--
 I also acknowledge that this approach swims against the DevSecOps tide in that it requires you to store your secrets (albeit encrypted)
 in Git, a practice that is often discouraged and typically forbidden at most organizations.
```

