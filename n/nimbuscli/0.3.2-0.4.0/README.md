# Comparing `tmp/nimbuscli-0.3.2.tar.gz` & `tmp/nimbuscli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbuscli-0.3.2.tar", max compression
+gzip compressed data, was "nimbuscli-0.4.0.tar", max compression
```

## Comparing `nimbuscli-0.3.2.tar` & `nimbuscli-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,48 @@
--rw-r--r--   0        0        0     1076 2024-05-05 12:53:29.436983 nimbuscli-0.3.2/LICENSE
--rw-r--r--   0        0        0     5027 2024-05-05 12:53:29.436983 nimbuscli-0.3.2/README.md
--rw-r--r--   0        0        0     2339 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/__init__.py
--rw-r--r--   0        0        0      132 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/__init__.py
--rw-r--r--   0        0        0     1523 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/factory.py
--rw-r--r--   0        0        0     1356 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/parser.py
--rw-r--r--   0        0        0     1189 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cli/runner.py
--rw-r--r--   0        0        0      209 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/__init__.py
--rw-r--r--   0        0        0     5528 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/backup.py
--rw-r--r--   0        0        0     3118 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/command.py
--rw-r--r--   0        0        0     3131 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/deploy.py
--rw-r--r--   0        0        0     4471 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/cmd/factory.py
--rw-r--r--   0        0        0     5473 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/config.py
--rw-r--r--   0        0        0      314 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/__init__.py
--rw-r--r--   0        0        0     4585 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/archiver.py
--rw-r--r--   0        0        0     3783 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/runner.py
--rw-r--r--   0        0        0     3102 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/service.py
--rw-r--r--   0        0        0     6727 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/core/uploader.py
--rw-r--r--   0        0        0     2333 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/log.py
--rw-r--r--   0        0        0     4642 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/main.py
--rw-r--r--   0        0        0      192 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/__init__.py
--rw-r--r--   0        0        0     4770 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/discord.py
--rw-r--r--   0        0        0     1191 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/factory.py
--rw-r--r--   0        0        0     1043 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/notify/notifier.py
--rw-r--r--   0        0        0      326 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/__init__.py
--rw-r--r--   0        0        0      758 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/directory.py
--rw-r--r--   0        0        0     2084 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/resource.py
--rw-r--r--   0        0        0     1868 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/secret.py
--rw-r--r--   0        0        0     3322 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/provider/service.py
--rw-r--r--   0        0        0      208 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/__init__.py
--rw-r--r--   0        0        0     2843 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/factory.py
--rw-r--r--   0        0        0     5712 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/format.py
--rw-r--r--   0        0        0    17618 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/reporter.py
--rw-r--r--   0        0        0     5275 2024-05-05 12:53:29.440983 nimbuscli-0.3.2/src/nimbuscli/report/writer.py
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 nimbuscli-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-30 17:04:31.238744 nimbuscli-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11805 2024-05-30 17:04:31.238744 nimbuscli-0.4.0/README.md
+-rw-r--r--   0        0        0     2339 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cli/__init__.py
+-rw-r--r--   0        0        0     1523 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cli/factory.py
+-rw-r--r--   0        0        0     1359 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cli/parser.py
+-rw-r--r--   0        0        0     1189 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cli/runner.py
+-rw-r--r--   0        0        0      209 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cmd/__init__.py
+-rw-r--r--   0        0        0     5539 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cmd/backup.py
+-rw-r--r--   0        0        0     3118 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cmd/command.py
+-rw-r--r--   0        0        0     3138 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cmd/deploy.py
+-rw-r--r--   0        0        0     4876 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/cmd/factory.py
+-rw-r--r--   0        0        0       72 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/config/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/config/config.py
+-rw-r--r--   0        0        0     3725 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/config/schema.py
+-rw-r--r--   0        0        0        0 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/__init__.py
+-rw-r--r--   0        0        0      241 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/archive/__init__.py
+-rw-r--r--   0        0        0     3686 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/archive/archiver.py
+-rw-r--r--   0        0        0     3702 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/archive/rar.py
+-rw-r--r--   0        0        0     1658 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/archive/tar.py
+-rw-r--r--   0        0        0     1687 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/archive/zip.py
+-rw-r--r--   0        0        0      122 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/deploy/__init__.py
+-rw-r--r--   0        0        0     1911 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/deploy/docker.py
+-rw-r--r--   0        0        0     1330 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/deploy/service.py
+-rw-r--r--   0        0        0      127 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/execute/__init__.py
+-rw-r--r--   0        0        0     2039 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/execute/process.py
+-rw-r--r--   0        0        0     2029 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/execute/runner.py
+-rw-r--r--   0        0        0      132 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/upload/__init__.py
+-rw-r--r--   0        0        0     4409 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/upload/aws.py
+-rw-r--r--   0        0        0     2506 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/core/upload/uploader.py
+-rw-r--r--   0        0        0     2333 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/log.py
+-rw-r--r--   0        0        0     4642 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/main.py
+-rw-r--r--   0        0        0      192 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/notify/__init__.py
+-rw-r--r--   0        0        0     4792 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/notify/discord.py
+-rw-r--r--   0        0        0     1191 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/notify/factory.py
+-rw-r--r--   0        0        0     1043 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/notify/notifier.py
+-rw-r--r--   0        0        0      326 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/provider/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/provider/directory.py
+-rw-r--r--   0        0        0     2084 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/provider/resource.py
+-rw-r--r--   0        0        0     1868 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/provider/secret.py
+-rw-r--r--   0        0        0     3371 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/provider/service.py
+-rw-r--r--   0        0        0      208 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/report/__init__.py
+-rw-r--r--   0        0        0     2843 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/report/factory.py
+-rw-r--r--   0        0        0     5715 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/report/format.py
+-rw-r--r--   0        0        0    17841 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/report/reporter.py
+-rw-r--r--   0        0        0     5275 2024-05-30 17:04:31.242744 nimbuscli-0.4.0/src/nimbuscli/report/writer.py
+-rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 nimbuscli-0.4.0/PKG-INFO
```

### Comparing `nimbuscli-0.3.2/LICENSE` & `nimbuscli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/pyproject.toml` & `nimbuscli-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nimbuscli"
-version = "0.3.2"
+version = "0.4.0"
 description = "Nimbus is engineered to optimize data backup processes and efficiently orchestrate service deployments."
 repository = "https://github.com/weak-head/nimbus"
 keywords = ["backup", "deploy", "administration"]
 authors = ["Oleksandr Zinchenko <zinchenko@live.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cli/factory.py` & `nimbuscli-0.4.0/src/nimbuscli/cli/factory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cli/parser.py` & `nimbuscli-0.4.0/src/nimbuscli/cli/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,11 +49,11 @@
 
     # -- Backup
     backup = commands.add_parser("backup")
     backup.add_argument(
         "selectors",
         nargs="*",
         default="",
-        help="glob patterns to filter folder groups",
+        help="glob patterns to filter directory groups",
     )
 
     return parser
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cli/runner.py` & `nimbuscli-0.4.0/src/nimbuscli/cli/runner.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cmd/backup.py` & `nimbuscli-0.4.0/src/nimbuscli/cmd/backup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,16 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 from logdecorator import log_on_end, log_on_start
 
 from nimbuscli.cmd.command import Action, ActionResult, Command
-from nimbuscli.core import (
-    ArchivalStatus,
-    Archiver,
-    Uploader,
-    UploadProgress,
-    UploadStatus,
-)
+from nimbuscli.core.archive import ArchivalStatus, Archiver
+from nimbuscli.core.upload import Uploader, UploadProgress, UploadStatus
 from nimbuscli.provider import DirectoryProvider, DirectoryResource
 
 
 class Backup(Command):
     """
     Create and upload backups.
     """
@@ -67,88 +62,91 @@
     def _backup(self, mapping: DirectoryMappingActionResult) -> BackupActionResult:
         result = BackupActionResult([])
 
         for group in mapping.entries:
             for directory in group.directories:
                 backup = BackupEntry(group.name, directory)
 
-                archive_path = self._compose_path(
+                archive_path = self._generate_backup_path(
                     self._destination,
                     backup.group,
-                    backup.folder,
-                    datetime.now(),
+                    backup.directory,
                 )
 
+                os.makedirs(os.path.dirname(archive_path), exist_ok=True)
+
                 backup.archive = self._archiver.archive(
-                    backup.folder,
+                    backup.directory,
                     archive_path,
                 )
 
                 result.entries.append(backup)
 
         return result
 
     def _upload(self, backups: BackupActionResult) -> UploadActionResult:
         result = UploadActionResult([])
 
         for backup in filter(lambda e: e.success, backups.entries):
             entry = UploadEntry(backup)
 
-            upload_key = self._compose_upload_key(
+            upload_key = self._generate_upload_key(
                 backup.group,
-                backup.folder,
+                backup.directory,
                 backup.archive.archive,
             )
 
             entry.upload = self._uploader.upload(
                 backup.archive.archive,
                 upload_key,
                 ProgressTracker(entry),
             )
 
             result.entries.append(entry)
 
         return result
 
-    def _compose_path(self, destination: str, group: str, folder: str, today: datetime) -> str:
-        suffix = 0
-        today_path = today.strftime("%Y-%m-%d_%H%M")
-        archive_name = Path(folder).name
-        base_path = os.path.join(destination, group, archive_name, f"{archive_name}_{today_path}")
+    def _generate_backup_path(self, destination: str, group: str, directory: str) -> str:
+        now = datetime.now().strftime("%Y-%m-%d_%H%M")
+        name = Path(directory).name
+        base_path = os.path.join(destination, group, name, f"{name}_{now}")
+        archive = f"{base_path}.{self._archiver.extension}"
 
         # Don't overwrite the existing backups under the same path.
         # Find the next available name that matches the pattern.
-        while True:
-            archive_path = base_path + (f"_{suffix:02d}.rar" if suffix > 0 else ".rar")
-            if os.path.exists(archive_path):
-                suffix += 1
-            else:
-                return archive_path
-
-    def _compose_upload_key(self, group: str, directory: str, archive: str) -> str:
-        directory_name = Path(directory).name
-        archive_name = Path(archive).name
-        return os.path.join(group, directory_name, archive_name)
+        suffix = 1
+        while os.path.exists(archive):
+            archive = f"{base_path}_{suffix:02d}.{self._archiver.extension}"
+            suffix += 1
+
+        return archive
+
+    def _generate_upload_key(self, group: str, directory: str, archive: str) -> str:
+        return os.path.join(
+            group,
+            Path(directory).name,
+            Path(archive).name,
+        )
 
 
 class ProgressTracker:
 
     def __init__(self, upload: UploadEntry):
         self._upload = upload
 
     @log_on_start(logging.INFO, "Uploaded progress {progress.progress!s}%")
     def __call__(self, progress: UploadProgress):
         self._upload.progress.append(progress)
 
 
 class BackupEntry:
 
-    def __init__(self, group: str, folder: str):
+    def __init__(self, group: str, directory: str):
         self.group: str = group
-        self.folder: str = folder
+        self.directory: str = directory
         self.archive: ArchivalStatus = None
 
     @property
     def success(self) -> bool:
         return self.archive and self.archive.success
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cmd/command.py` & `nimbuscli-0.4.0/src/nimbuscli/cmd/command.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cmd/deploy.py` & `nimbuscli-0.4.0/src/nimbuscli/cmd/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from abc import abstractmethod
 from typing import Any
 
 from logdecorator import log_on_end
 
 from nimbuscli.cmd.command import Action, ActionResult, Command
-from nimbuscli.core import OperationStatus, Service
+from nimbuscli.core.deploy import OperationStatus, Service
 from nimbuscli.provider import ServiceFactory, ServiceProvider, ServiceResource
 
 
 class Deployment(Command):
     """
     Manage service deployment.
     """
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/cmd/factory.py` & `nimbuscli-0.4.0/src/nimbuscli/cmd/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,17 @@
 
 from logdecorator import log_on_end, log_on_error, log_on_start
 
 from nimbuscli.cmd.backup import Backup
 from nimbuscli.cmd.command import Command
 from nimbuscli.cmd.deploy import Down, Up
 from nimbuscli.config import Config
-from nimbuscli.core import (
-    Archiver,
-    AwsUploader,
-    RarArchiver,
-    SubprocessRunner,
-    Uploader,
-)
+from nimbuscli.core.archive import Archiver, RarArchiver, TarArchiver, ZipArchiver
+from nimbuscli.core.execute import SubprocessRunner
+from nimbuscli.core.upload import AwsUploader, Uploader
 from nimbuscli.provider import (
     DirectoryProvider,
     Secrets,
     SecretsProvider,
     ServiceFactory,
     ServiceProvider,
 )
@@ -43,14 +39,19 @@
         pass
 
 
 class CfgCommandFactory(CommandFactory):
 
     def __init__(self, config: Config) -> None:
         self._cfg = config
+        self._profiles = {
+            "rar": Config({"provider": "rar", "password": None, "compress": 3, "recovery": 3}),
+            "tar": Config({"provider": "tar", "compress": "xz"}),
+            "zip": Config({"provider": "zip", "compress": "xz"}),
+        }
 
     @log_on_start(logging.DEBUG, "Creating Backup command")
     @log_on_error(logging.ERROR, "Failed to create Backup command: {e!r}", on_exceptions=Exception)
     def create_backup(self, selectors: list[str]) -> Command:
         cfg = self._cfg.commands.backup
         return Backup(
             selectors,
@@ -78,36 +79,43 @@
             self.create_service_factory(),
         )
 
     @log_on_start(logging.DEBUG, "Creating Archiver: [{profile!s}]")
     @log_on_end(logging.DEBUG, "Created Archiver: {result!r}")
     @log_on_error(logging.ERROR, "Failed to create Archiver: {e!r}", on_exceptions=Exception)
     def create_archiver(self, profile: str) -> Archiver:
-        if cfg := CfgCommandFactory._profile(self._cfg.profiles.archive, profile):
-            if cfg.provider == "rar":
-                return RarArchiver(
-                    SubprocessRunner(),
-                    cfg.password,
-                    cfg.compression,
-                    cfg.recovery,
-                )
+        # Load the archive profile from the app config
+        p = self._cfg.first("profiles.archive", lambda x: x.name == profile)
+
+        # Try to load a default profile
+        if p is None:
+            p = self._profiles.get(profile, None)
+
+        if p is not None:
+            match p.provider:
+                case "rar":
+                    return RarArchiver(SubprocessRunner(), p.password, p.compress, p.recovery)
+                case "tar":
+                    return TarArchiver(p.compress)
+                case "zip":
+                    return ZipArchiver(p.compress)
 
         return None
 
     @log_on_start(logging.DEBUG, "Creating Uploader: [{profile!s}]")
     @log_on_end(logging.DEBUG, "Created Uploader: {result!r}")
     @log_on_error(logging.ERROR, "Failed to create Uploader: {e!r}", on_exceptions=Exception)
     def create_uploader(self, profile: str) -> Uploader:
-        if cfg := CfgCommandFactory._profile(self._cfg.profiles.upload, profile):
+        if cfg := self._cfg.first("profiles.upload", lambda x: x.name == profile):
             if cfg.provider == "aws":
                 return AwsUploader(
                     cfg.access_key,
                     cfg.secret_key,
                     cfg.bucket,
-                    cfg.storage_class,
+                    cfg.storage,
                 )
 
         return None
 
     @log_on_start(logging.DEBUG, "Creating Service Provider")
     @log_on_end(logging.DEBUG, "Created Service Provider: {result!r}")
     @log_on_error(logging.ERROR, "Failed to create Service Provider: {e!r}", on_exceptions=Exception)
@@ -118,13 +126,7 @@
     @log_on_end(logging.DEBUG, "Created Service Factory: {result!r}")
     @log_on_error(logging.ERROR, "Failed to create Service Factory: {e!r}", on_exceptions=Exception)
     def create_service_factory(self) -> ServiceFactory:
         return ServiceFactory(
             SubprocessRunner(),
             Secrets(SecretsProvider(self._cfg.commands.deploy.secrets)),
         )
-
-    @staticmethod
-    def _profile(profiles: list[Config], name: str) -> Config | None:
-        if cfg := [c for c in profiles if c.name == name]:
-            return cfg[0]
-        return None
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/core/archiver.py` & `nimbuscli-0.4.0/src/nimbuscli/core/archive/rar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,18 @@
-from __future__ import annotations
-
 import logging
-import os
-from abc import ABC, abstractmethod
 
 from logdecorator import log_on_end, log_on_start
 
-from nimbuscli.core.runner import CompletedProcess, Runner
-
-
-class Archiver(ABC):
-    """
-    Defines an abstract archiver.
-    All archivers should follow the APIs defined by this class.
-    """
-
-    @abstractmethod
-    def archive(self, folder: str, archive: str) -> ArchivalStatus:
-        """
-        Archive a folder.
-
-        :param folder: Full path to the folder that should be archived.
-        :param archive: A file path where the archive should be created.
-        :return: Status of the folder archival.
-        """
-
-
-class ArchivalStatus:
-
-    def __init__(self, proc: CompletedProcess, folder: str, archive: str):
-        self.proc = proc
-        self.folder = folder
-        self.archive = archive
-
-    @property
-    def success(self) -> bool:
-        return all(
-            [
-                self.proc.success,
-                self.folder,
-                self.archive,
-                os.path.exists(self.archive),
-            ]
-        )
-
-    @property
-    def size(self) -> int:
-        return os.stat(self.archive).st_size if self.success else None
-
-    @property
-    def speed(self) -> int:
-        return int(self.size // self.proc.elapsed.total_seconds()) if self.success else 0
+from nimbuscli.core.archive.archiver import ArchivalStatus, Archiver
+from nimbuscli.core.execute import CompletedProcess, Runner
 
 
 class RarArchiver(Archiver):
     """
-    Create a password protected archive using 'WinRar'.
+    Creates a password protected archive using 'WinRar'.
     https://www.win-rar.com/download.html
     """
 
     def __init__(
         self,
         runner: Runner,
         password: str | None = None,
@@ -73,25 +26,22 @@
         :param password: Password to protect the archive with.
         :param compression: Compression level [0-5].
         :param recovery: Recovery record (%) [0-1000].
         """
         if runner is None:
             raise ValueError("The runner cannot be None")
 
-        if password is not None:
-            if password == "":
-                raise ValueError("If password is specified, it cannot be empty string")
-
-        if compression is not None:
-            if not 0 <= compression <= 5:
-                raise ValueError("Compression should be in range [0-5]")
-
-        if recovery is not None:
-            if not 0 <= recovery <= 1000:
-                raise ValueError("Recovery should be in range [0-1000]")
+        if password is not None and password == "":
+            raise ValueError("If password is specified, it cannot be empty string.")
+
+        if compression is not None and not 0 <= compression <= 5:
+            raise ValueError("Compression should be either None or in [0-5] range.")
+
+        if recovery is not None and not 0 <= recovery <= 1000:
+            raise ValueError("Recovery should be either None or in [0-1000] range.")
 
         self._runner = runner
         self._password = password
         self._compression = compression
         self._recovery = recovery
 
     def __repr__(self) -> str:
@@ -99,28 +49,28 @@
             f"'{self._runner.__class__.__name__}'",
             f"pwd='{self._password}'",
             f"cmp='{self._compression}'",
             f"rec='{self._recovery}'",
         ]
         return "RarArchiver(" + ", ".join(params) + ")"
 
-    @log_on_start(logging.INFO, "Archiving {folder!s} -> {archive!s}")
-    @log_on_end(logging.INFO, "Archived [{result.success!s}]: {archive!s}")
-    def archive(self, folder: str, archive: str) -> ArchivalStatus:
-        # Ensure destination folder exists
-        directory_path = os.path.dirname(archive)
-        if not os.path.exists(directory_path):
-            os.makedirs(directory_path, exist_ok=True)
+    @property
+    def extension(self) -> str:
+        return "rar"
 
+    @log_on_start(logging.INFO, "Archiving {directory!s} -> {archive!s}")
+    @log_on_end(logging.INFO, "Archived [{result.success!s}]: {archive!s}")
+    def archive(self, directory: str, archive: str) -> ArchivalStatus:
         # It is expected that 'rar' executable
         # is available in a system PATH.
-        proc = self._runner.execute(self._build_cmd(folder, archive))
-        return ArchivalStatus(proc, folder, archive)
+        cmd = self._generate_cmd(directory, archive)
+        proc = self._runner.execute(cmd)
+        return RarArchivalStatus(proc, directory, archive)
 
-    def _build_cmd(self, folder: str, archive: str) -> list[str]:
+    def _generate_cmd(self, directory: str, archive: str) -> list[str]:
         # fmt: off
         cmd = [
             "rar",
             "a",        # Archive
             "-r",       # Recursive
             "-ol",      # Process symbolic links as the link
             "-htb",     # Use BLAKE2 hash
@@ -141,9 +91,22 @@
         if self._compression is not None:
             cmd.append(f"-m{self._compression}")
 
         # Protect with password
         if self._password is not None:
             cmd.append(f"-hp{self._password}")
 
-        cmd.extend([archive, folder])
+        cmd.extend([archive, directory])
         return cmd
+
+
+class RarArchivalStatus(ArchivalStatus):
+
+    def __init__(self, proc: CompletedProcess, directory: str, archive: str):
+        super().__init__(directory, archive)
+        self.started = proc.started
+        self.completed = proc.completed
+        self.proc = proc
+
+    @property
+    def success(self) -> bool:
+        return all([self.proc.success, super().success])
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/core/service.py` & `nimbuscli-0.4.0/src/nimbuscli/core/deploy/docker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,15 @@
 from __future__ import annotations
 
 import logging
-from abc import ABC, abstractmethod
-from datetime import timedelta
-from functools import reduce
 
 from logdecorator import log_on_end, log_on_start
 
-from nimbuscli.core.runner import CompletedProcess, Runner
-
-
-class Service(ABC):
-    """
-    Defines an abstract service.
-    All services should follow the APIs defined by this class.
-    """
-
-    def __init__(self, name: str):
-        self._name: str = name
-
-    def __str__(self) -> str:
-        return self.name
-
-    @property
-    def name(self) -> str:
-        """
-        Service name.
-        """
-        return self._name
-
-    @abstractmethod
-    def start(self) -> OperationStatus:
-        """
-        Start the service.
-        """
-
-    @abstractmethod
-    def stop(self) -> OperationStatus:
-        """
-        Stop the service.
-        """
-
-
-class OperationStatus:
-    """
-    The outcome of the service operation.
-    """
-
-    def __init__(self, service: str, operation: str, kind: str):
-        self.service: str = service
-        self.operation: str = operation
-        self.kind: str = kind
-        self.processes: list[CompletedProcess] = []
-
-    @property
-    def success(self) -> bool:
-        return all(proc.success for proc in self.processes)
-
-    @property
-    def elapsed(self) -> timedelta:
-        return reduce(lambda a, b: a + b.elapsed, self.processes, timedelta(seconds=0))
+from nimbuscli.core.deploy.service import OperationStatus, Service
+from nimbuscli.core.execute import Runner
 
 
 class DockerService(Service):
     """
     A Dockerized service orchestrated using a docker-compose file.
     """
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/core/uploader.py` & `nimbuscli-0.4.0/src/nimbuscli/core/upload/aws.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,19 @@
 from __future__ import annotations
 
 import logging
 import os
 import threading
-from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 from typing import Callable
 
 from boto3 import Session
 from logdecorator import log_on_end, log_on_error, log_on_start
 
-
-class Uploader(ABC):
-    """
-    Defines an abstract file uploader.
-    All uploaders should follow the APIs defined by this class.
-    """
-
-    @abstractmethod
-    def config(self) -> dict[str, str]:
-        """
-        Returns a configuration used by this uploader.
-        """
-
-    @abstractmethod
-    def upload(
-        self,
-        filepath: str,
-        key: str,
-        on_progress: Callable[[UploadProgress], None] = None,
-    ) -> UploadStatus:
-        """
-        Upload a file to the pre-configured destination.
-
-        :param filepath: Full path to the file that should be uploaded.
-        :param key: The name of the key to upload to.
-        :param on_progress: An optional callback that is invoked on progress update.
-        :return: Status of the file upload.
-        """
-
-
-class UploadProgress:
-    """
-    Defines a file upload progress.
-    """
-
-    def __init__(self, progress: int, elapsed: timedelta, speed: int):
-        self.progress = progress
-        self.elapsed = elapsed
-        self.speed = speed
-        self.timestamp = datetime.now()
-
-    def __repr__(self):
-        params = [
-            f"timestamp='{self.timestamp}'",
-            f"progress='{self.progress}'",
-            f"speed='{self.speed}'",
-            f"elapsed='{self.elapsed}'",
-        ]
-        return "UploadProgress(" + ", ".join(params) + ")"
-
-
-class UploadStatus:
-
-    SUCCESS = "success"
-    FAILED = "failed"
-
-    def __init__(self, filepath: str, key: str):
-        self.filepath: str = filepath
-        self.key: str = key
-        self.size: int = None
-        self.started: datetime = None
-        self.completed: datetime = None
-        self.exception: Exception = None
-
-    @property
-    def status(self) -> str:
-        return UploadStatus.FAILED if self.exception else UploadStatus.SUCCESS
-
-    @property
-    def success(self) -> bool:
-        return all(
-            [
-                self.status == UploadStatus.SUCCESS,
-                self.filepath,
-                self.key,
-                self.size,
-                self.started,
-                self.completed,
-            ]
-        )
-
-    @property
-    def elapsed(self) -> timedelta:
-        return max(timedelta(seconds=1), self.completed - self.started)
-
-    @property
-    def speed(self) -> int:
-        return int(self.size // self.elapsed.total_seconds()) if self.success else 0
+from nimbuscli.core.upload.uploader import Uploader, UploadProgress, UploadStatus
 
 
 class AwsUploader(Uploader):
     """
     Upload files to AWS S3 bucket.
     """
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/log.py` & `nimbuscli-0.4.0/src/nimbuscli/log.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/main.py` & `nimbuscli-0.4.0/src/nimbuscli/main.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/notify/discord.py` & `nimbuscli-0.4.0/src/nimbuscli/notify/discord.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,42 +15,47 @@
     Sends notifications to a Discord channel.
     """
 
     _FAILURE = 0xFF0000
     _SUCCESS = 0x00FF00
 
     def __init__(self, webhook: str, username: str = None, avatar_url: str = None) -> None:
+        """
+        Creates a new instance of the DiscordNotifier.
+
+        :param webhook: Discord webhook url.
+        :param username: Overwrite username (optional).
+        :param avatar_url: Overwrite avatar (optional).
+        """
+        if not webhook:
+            raise ValueError("The webhook cannot be None or empty.")
+
         self._webhook = webhook
         self._username = username
         self._avatar_url = avatar_url
 
     def __repr__(self) -> str:
         params = [
             f"webhook='{self._webhook}'",
             f"username='{self._username}'",
             f"avatar_url='{self._avatar_url}'",
         ]
         return "DiscordNotifier(" + ", ".join(params) + ")"
 
-    def _send_message(self, json: dict) -> None:
-        requests.post(
-            self._webhook,
-            json=json,
-            timeout=3_000,
-        )
-
-    def _send_attachment(self, filepath: str) -> None:
-        with open(filepath, "rb") as file:
-            requests.post(
-                self._webhook,
-                files={"file": file},
-                timeout=10_000,
-            )
+    def completed(self, result: ExecutionResult, attachments: list[str] = None) -> None:
+        requests.post(self._webhook, json=self.compose_request(result), timeout=3_000)
 
-    def _compose_completed(self, result: ExecutionResult) -> dict:
+        if not attachments:
+            return
+
+        for attachment in attachments:
+            with open(attachment, "rb") as file:
+                requests.post(self._webhook, files={"file": file}, timeout=10_000)
+
+    def compose_request(self, result: ExecutionResult) -> dict:
         """
         Compose 'completed' notification request that follows the discord spec:
             - https://discord.com/developers/docs/resources/webhook
         """
         data = {}
         if self._username:
             data["username"] = self._username
@@ -61,62 +66,64 @@
         event["title"] = f"{fmt.ch('success') if result.success else fmt.ch('failure')} {result.command}"
         event["color"] = DiscordNotifier._SUCCESS if result.success else DiscordNotifier._FAILURE
         event["timestamp"] = datetime.now().astimezone().isoformat()
         event["fields"] = [
             {"name": f"{fmt.ch('duration')} Elapsed", "value": f"{fmt.duration(result.elapsed)}", "inline": True},
             {"name": f"{fmt.ch('time')} Started", "value": f"{fmt.datetime(result.started)}", "inline": True},
             {"name": f"{fmt.ch('time')} Completed", "value": f"{fmt.datetime(result.completed)}", "inline": True},
-            *self._details(result),
+            *self._execution_details(result),
         ]
 
         data["embeds"] = [event]
         return data
 
-    def _details(self, result: ExecutionResult) -> Iterator[dict]:
+    def _execution_details(self, result: ExecutionResult) -> Iterator[dict]:
         for action in result.actions:
             match action:
                 case DeploymentActionResult():
-                    yield {
-                        "name": f"{fmt.ch('service')} Services",
-                        "value": "\n".join(
-                            [
-                                f"{ix:02d}. "
-                                f"{fmt.ch('success') if entry.success else fmt.ch('failure')} "
-                                f"{fmt.ch(entry.kind)} {entry.service}"
-                                for ix, entry in enumerate(action.entries)
-                            ]
-                        ),
-                        "inline": False,
-                    }
+                    yield self._deployment_details(action)
                 case BackupActionResult():
-                    yield {
-                        "name": f"{fmt.ch('backup')} Backups",
-                        "value": "\n".join(
-                            [
-                                f"{ix:02d}. "
-                                f"{fmt.ch('success') if entry.success else fmt.ch('failure')} "
-                                f"{fmt.ch('folder')} {entry.folder}"
-                                for ix, entry in enumerate(action.entries)
-                            ]
-                        ),
-                        "inline": False,
-                    }
+                    yield self._backup_details(action)
                 case UploadActionResult():
-                    yield {
-                        "name": f"{fmt.ch('upload')} Uploads",
-                        "value": "\n".join(
-                            [
-                                f"{ix:02d}. "
-                                f"{fmt.ch('success') if entry.success else fmt.ch('failure')} "
-                                f"{fmt.ch('archive')} {entry.upload.key}"
-                                for ix, entry in enumerate(action.entries)
-                            ]
-                        ),
-                        "inline": False,
-                    }
-
-    def completed(self, result: ExecutionResult, attachments: list[str] = None) -> None:
-        self._send_message(self._compose_completed(result))
+                    yield self._upload_details(action)
 
-        if attachments is not None:
-            for attachment in attachments:
-                self._send_attachment(attachment)
+    def _deployment_details(self, action: DeploymentActionResult) -> dict:
+        return {
+            "name": f"{fmt.ch('service')} Services",
+            "value": "\n".join(
+                [
+                    f"{ix:02d}. "
+                    f"{fmt.ch('success') if entry.success else fmt.ch('failure')} "
+                    f"{fmt.ch(entry.kind)} {entry.service}"
+                    for ix, entry in enumerate(action.entries)
+                ]
+            ),
+            "inline": False,
+        }
+
+    def _backup_details(self, action: BackupActionResult) -> dict:
+        return {
+            "name": f"{fmt.ch('backup')} Backups",
+            "value": "\n".join(
+                [
+                    f"{ix:02d}. "
+                    f"{fmt.ch('success') if entry.success else fmt.ch('failure')} "
+                    f"{fmt.ch('directory')} {entry.directory}"
+                    for ix, entry in enumerate(action.entries)
+                ]
+            ),
+            "inline": False,
+        }
+
+    def _upload_details(self, action: UploadActionResult) -> dict:
+        return {
+            "name": f"{fmt.ch('upload')} Uploads",
+            "value": "\n".join(
+                [
+                    f"{ix:02d}. "
+                    f"{fmt.ch('success') if entry.success else fmt.ch('failure')} "
+                    f"{fmt.ch('archive')} {entry.upload.key}"
+                    for ix, entry in enumerate(action.entries)
+                ]
+            ),
+            "inline": False,
+        }
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/notify/factory.py` & `nimbuscli-0.4.0/src/nimbuscli/notify/factory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/notify/notifier.py` & `nimbuscli-0.4.0/src/nimbuscli/notify/notifier.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/provider/directory.py` & `nimbuscli-0.4.0/src/nimbuscli/provider/directory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/provider/resource.py` & `nimbuscli-0.4.0/src/nimbuscli/provider/resource.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/provider/secret.py` & `nimbuscli-0.4.0/src/nimbuscli/provider/secret.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/provider/service.py` & `nimbuscli-0.4.0/src/nimbuscli/provider/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import logging
 from pathlib import Path
 from typing import Iterator
 
 from logdecorator import log_on_end, log_on_error, log_on_start
 
-from nimbuscli.core import DockerService, Runner, Service
+from nimbuscli.core.deploy import DockerService, Service
+from nimbuscli.core.execute import Runner
 from nimbuscli.provider.resource import Provider, Resource
 from nimbuscli.provider.secret import Secrets
 
 
 class ServiceResource(Resource):
 
     def __init__(self, name: str, kind: str, directory: str):
@@ -18,16 +19,16 @@
         self.kind: str = kind
         self.directory: str = directory
 
 
 class ServiceProvider(Provider[ServiceResource]):
     """
     This class provides a recursive mechanism for
-    discovering services within all parent folders.
-    By traversing through parent folders, it facilitates
+    discovering services within all parent directories.
+    By traversing through parent directories, it facilitates
     the identification and interaction with services,
     """
 
     def __init__(self, directories: list[str]):
         self._directories: list[str] = directories
         self._compose_files = [
             "compose.yml",
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/report/factory.py` & `nimbuscli-0.4.0/src/nimbuscli/report/factory.py`

 * *Files identical despite different names*

### Comparing `nimbuscli-0.3.2/src/nimbuscli/report/format.py` & `nimbuscli-0.4.0/src/nimbuscli/report/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     to the corresponding Unicode character representation.
     """
     m = {
         # -- Reporting --
         "summary": "📄️",  # 📋
         "details": "🔍",
         "cloud": "☁️",
-        "folder": "📁",
+        "directory": "📁",
         "mapping": "🗺️",
         "backup": "💼",  # 🗂️ 📀 💿 💾 🗜️ 🗃️ 💼 ⚙️ 🔨 🔧
         "upload": "⬆️",
         "download": "⬇️",
         "exception": "⚠️",  # 🛑
         "exitcode": "❗",
         "outgoing": "📤",
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/report/reporter.py` & `nimbuscli-0.4.0/src/nimbuscli/report/reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     UploadActionResult,
 )
 from nimbuscli.cmd.deploy import (
     CreateServicesActionResult,
     DeploymentActionResult,
     ServiceMappingActionResult,
 )
+from nimbuscli.core.archive import RarArchivalStatus
 from nimbuscli.report.writer import Writer
 
 
 class Reporter(ABC):
 
     @abstractmethod
     def write(self, result: ExecutionResult) -> None:
@@ -161,15 +162,15 @@
         )
 
     def summary_backup(self, w: Writer, base: str, result: BackupActionResult) -> None:
         if created := sorted(
             (
                 b.archive.archive.replace(base, "")[1:],
                 fmt.size(b.archive.size),
-                fmt.duration(b.archive.proc.elapsed),
+                fmt.duration(b.archive.elapsed),
                 fmt.speed(b.archive.speed),
             )
             for b in result.entries
             if b.success
         ):
             b = w.section(
                 f"{fmt.ch('success')} Successful backups "
@@ -181,15 +182,15 @@
                     f"| {fmt.ch('duration')} {duration} "
                     f"| {fmt.ch('speed')} {speed} ]"
                     for name, size, duration, speed in fmt.align(created, "lrrr")
                 ],
                 style="number",
             )
 
-        if failed := sorted(f"{fmt.ch('folder')} {b.folder}" for b in result.entries if not b.success):
+        if failed := sorted(f"{fmt.ch('directory')} {b.directory}" for b in result.entries if not b.success):
             b = w.section(f"{fmt.ch('failure')} Failed backups -- ¯\\_(ツ)_/¯")
             b.list(failed, style="number")
 
     def summary_upload(self, w: Writer, result: UploadActionResult) -> None:
         if uploaded := sorted(
             (
                 e.upload.key,
@@ -258,51 +259,53 @@
         d.row("Success", f"{fmt.ch('success') if result.success else fmt.ch('failure')} {result.success}")
         d.row("Started", f"{fmt.ch('time')} {fmt.datetime(result.started)}")
         d.row("Completed", f"{fmt.ch('time')} {fmt.datetime(result.completed)}")
         d.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(result.elapsed)}")
 
         for group in sorted(result.entries, key=lambda e: e.name):
             g = d.section(f"Group [{group.name}]:")
-            g.list((f"{fmt.ch('folder')} {v}" for v in sorted(group.directories)))
+            g.list((f"{fmt.ch('directory')} {v}" for v in sorted(group.directories)))
 
     def details_backup(self, w: Writer, result: BackupActionResult):
         d = w.section(f"{fmt.ch('backup')} Backup")
         d.row("Success", f"{fmt.ch('success') if result.success else fmt.ch('failure')} {result.success}")
         d.row("Total Size", f"{fmt.ch('size')} {fmt.size(result.total_size)}")
         d.row("Started", f"{fmt.ch('time')} {fmt.datetime(result.started)}")
         d.row("Completed", f"{fmt.ch('time')} {fmt.datetime(result.completed)}")
         d.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(result.elapsed)}")
 
         total_backups = len(result.entries)
-        for ix, entry in enumerate(sorted(result.entries, key=lambda e: (e.group, e.folder))):
-            b = d.section(f"[{ix+1}/{total_backups}] [{entry.group}] {fmt.ch('folder')} {entry.folder}")
+        for ix, entry in enumerate(sorted(result.entries, key=lambda e: (e.group, e.directory))):
+            b = d.section(f"[{ix+1}/{total_backups}] [{entry.group}] {fmt.ch('directory')} {entry.directory}")
             b.row("Success", f"{fmt.ch('success') if entry.success else fmt.ch('failure')} {entry.success}")
-            b.row("Started", f"{fmt.ch('time')} {fmt.datetime(entry.archive.proc.started)}")
-            b.row("Completed", f"{fmt.ch('time')} {fmt.datetime(entry.archive.proc.completed)}")
-            b.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(entry.archive.proc.elapsed)}")
+            b.row("Started", f"{fmt.ch('time')} {fmt.datetime(entry.archive.started)}")
+            b.row("Completed", f"{fmt.ch('time')} {fmt.datetime(entry.archive.completed)}")
+            b.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(entry.archive.elapsed)}")
 
-            if entry.archive.proc.success:
+            if entry.archive.success:
                 b.row("Size", f"{fmt.ch('size')} {fmt.size(entry.archive.size)}")
                 b.row("Speed", f"{fmt.ch('speed')} {fmt.speed(entry.archive.speed)}")
                 b.row("Archive", f"{fmt.ch('archive')} {entry.archive.archive}")
             else:
-                if entry.archive.proc.exitcode:
-                    b.row("Exit Code", f"{fmt.ch('exitcode')} {entry.archive.proc.exitcode}")
-
-                if entry.archive.proc.stdout:
-                    s = b.section("StdOut", indent=False)
-                    s.list(entry.archive.proc.stdout.split("\n"))
-
-                if entry.archive.proc.stderr:
-                    s = b.section("StdErr", indent=False)
-                    s.list(entry.archive.proc.stderr.split("\n"))
-
-                if entry.archive.proc.exception:
-                    ex = b.section(f"{fmt.ch('exception')} Exception")
-                    ex.list(fmt.wrap(str(entry.archive.proc.exception)))
+                match entry.archive:
+                    case RarArchivalStatus():
+                        if entry.archive.proc.exitcode:
+                            b.row("Exit Code", f"{fmt.ch('exitcode')} {entry.archive.proc.exitcode}")
+
+                        if entry.archive.proc.stdout:
+                            s = b.section("StdOut", indent=False)
+                            s.list(entry.archive.proc.stdout.split("\n"))
+
+                        if entry.archive.proc.stderr:
+                            s = b.section("StdErr", indent=False)
+                            s.list(entry.archive.proc.stderr.split("\n"))
+
+                        if entry.archive.proc.exception:
+                            ex = b.section(f"{fmt.ch('exception')} Exception")
+                            ex.list(fmt.wrap(str(entry.archive.proc.exception)))
 
     def details_upload(self, w: Writer, result: UploadActionResult):
         d = w.section(f"{fmt.ch('upload')} Upload")
         d.row("Success", f"{fmt.ch('success') if result.success else fmt.ch('failure')} {result.success}")
         d.row("Total Size", f"{fmt.ch('size')} {fmt.size(result.total_size)}")
         d.row("Started", f"{fmt.ch('time')} {fmt.datetime(result.started)}")
         d.row("Completed", f"{fmt.ch('time')} {fmt.datetime(result.completed)}")
@@ -350,15 +353,15 @@
         s.row("Completed", f"{fmt.ch('time')} {fmt.datetime(result.completed)}")
         s.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(result.elapsed)}")
 
         mapping = sorted((e.name, e.directory, e.kind) for e in result.entries)
         g = s.section(f"{fmt.ch('service')} Services")
         g.list(
             [
-                f"{fmt.ch(kind)} {name} | {fmt.ch('folder')} {directory}"
+                f"{fmt.ch(kind)} {name} | {fmt.ch('directory')} {directory}"
                 for name, directory, kind in fmt.align(mapping, "llr")
             ],
         )
 
     def details_create_services(self, w: Writer, result: CreateServicesActionResult):
         pass
 
@@ -382,15 +385,15 @@
                 f"{fmt.ch('time')} {fmt.datetime(max(t.completed for e in result.entries for t in e.processes))}",
             )
             b.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(entry.elapsed)}")
 
             for proc in entry.processes:
                 p = b.section(f"{fmt.ch('shell')} {' '.join(proc.cmd)}")
                 p.row("Success", f"{fmt.ch('success') if proc.success else fmt.ch('failure')} {proc.success}")
-                p.row("Directory", f"{fmt.ch('folder')} {proc.cwd}")
+                p.row("Directory", f"{fmt.ch('directory')} {proc.cwd}")
                 p.row("Started", f"{fmt.ch('time')} {fmt.datetime(proc.started)}")
                 p.row("Completed", f"{fmt.ch('time')} {fmt.datetime(proc.completed)}")
                 p.row("Elapsed", f"{fmt.ch('duration')} {fmt.duration(proc.elapsed)}")
 
                 if proc.exitcode:
                     p.row("Exit Code", f"{fmt.ch('exitcode')} {proc.exitcode}")
```

### Comparing `nimbuscli-0.3.2/src/nimbuscli/report/writer.py` & `nimbuscli-0.4.0/src/nimbuscli/report/writer.py`

 * *Files identical despite different names*

