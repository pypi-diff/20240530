# Comparing `tmp/btrview-0.7.2.tar.gz` & `tmp/btrview-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.7.2.tar", last modified: Mon May 27 14:56:52 2024, max compression
+gzip compressed data, was "btrview-0.8.0.tar", last modified: Wed May 29 20:36:19 2024, max compression
```

## Comparing `btrview-0.7.2.tar` & `btrview-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.7.2/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-27 14:56:52.147232 btrview-0.7.2/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4352 2024-05-09 03:55:16.000000 btrview-0.7.2/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       88 2024-05-27 14:56:48.000000 btrview-0.7.2/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7839 2024-05-27 14:55:48.000000 btrview-0.7.2/btrview/btrfs.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/rich_output.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/btrview/scripts/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4534 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3462 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/typed_info.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1278 2024-05-27 14:31:43.000000 btrview-0.7.2/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      390 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-27 14:56:48.000000 btrview-0.7.2/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-27 14:56:52.147232 btrview-0.7.2/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-29 20:36:19.085212 btrview-0.8.0/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.8.0/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     7412 2024-05-29 20:36:19.081879 btrview-0.8.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     5400 2024-05-29 20:33:41.000000 btrview-0.8.0/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-29 20:36:19.081879 btrview-0.8.0/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       88 2024-05-29 20:09:41.000000 btrview-0.8.0/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2177 2024-05-29 20:03:44.000000 btrview-0.8.0/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6987 2024-05-29 19:59:34.000000 btrview-0.8.0/btrview/btrfs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6912 2024-05-29 19:59:34.000000 btrview-0.8.0/btrview/rich_output.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-29 20:36:19.081879 btrview-0.8.0/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2177 2024-05-29 20:03:44.000000 btrview-0.8.0/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     5319 2024-05-28 17:35:34.000000 btrview-0.8.0/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3487 2024-05-28 17:35:34.000000 btrview-0.8.0/btrview/typed_info.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     2167 2024-05-29 19:59:34.000000 btrview-0.8.0/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-29 20:36:19.081879 btrview-0.8.0/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     7412 2024-05-29 20:36:19.000000 btrview-0.8.0/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      390 2024-05-29 20:36:19.000000 btrview-0.8.0/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-29 20:36:19.000000 btrview-0.8.0/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-29 20:36:19.000000 btrview-0.8.0/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-29 20:36:19.000000 btrview-0.8.0/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-29 20:36:19.000000 btrview-0.8.0/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-29 20:09:41.000000 btrview-0.8.0/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-29 20:36:19.085212 btrview-0.8.0/setup.cfg
```

### Comparing `btrview-0.7.2/LICENSE.md` & `btrview-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.7.2/PKG-INFO` & `btrview-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.7.2
+Version: 0.8.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,23 +58,31 @@
 Subvolumes that are mounted (in fstab or somehow else) are in bold, those that are grey are subvolumes that aren't currently reachable on the filesystem, and subvolumes in red (not shown here) are not currently on the filesytem. This could be because they're deleted, or maybe its child subvolume was `btrfs received` from another filesystem.
 
 Wondering what the difference between the subvolume and snapshot tree is? [Check out the FAQ](#q-whats-the-difference-between-the-subvolume-tree-and-the-snapshot-tree)!
 
 ## Installation:
 
 Btrview relies on the following dependencies:
-* python 3.11 or greater
-* btrfs-progs
-* python-treelib
-* python-rich
+* [python 3.11 or greater](https://www.python.org/)
+* [findmnt](https://man7.org/linux/man-pages/man8/findmnt.8.html) (should be installed by default on most distributions)
+* [btrfs-progs](https://github.com/kdave/btrfs-progs/tree/master)
+* [python-btrfsutil](https://github.com/kdave/btrfs-progs/tree/master/libbtrfsutil) (might be included with btrfs progs)
+* [python-treelib](https://treelib.readthedocs.io/en/latest/)
+* [python-rich](https://rich.readthedocs.io/en/stable/introduction.html)
 
-The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx install --system-site-packages btrview`. Using pipx to install btrview will also install the required python dependencies and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
+The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx install --system-site-packages btrview`. Using pipx to install btrview will also install treelib and rich and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
 
 If you don't feel like installing via pipx you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
 
+### Installation Troubleshooting
+
+Q: How come when I use the sudo command with btrview I get `sudo: btrview: command not found`, but when I run it without sudo the command is recognized?
+
+A: You are likely are using a linux distribution which hard codes the paths sudo can use to find executables. There are one of two options here, you can either comment out the line that contains "secure_path" in `/etc/sudoers` or you can add the path you're using to that variable. The former option will change it so that any executable in the user's path can be executed, the latter option will merely add the user's path to list of allowed paths.
+
 ## Some Qs and As:
 
 ### Q: What is btrfs?
 
 In short, it's a copy on write (COW) filesystem. If you're not already using btrfs, then check out the [documentation](https://btrfs.readthedocs.io/en/latest/) to see if it's something you'd be interested in.
 
 ### Q: What does btrview do?
```

### Comparing `btrview-0.7.2/btrview/__main__.py` & `btrview-0.8.0/btrview/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import argparse
 
 import btrview
 from btrview.utils import check_root
-from btrview.rich_output import logic,SORT_FUNCS
-from btrview.btrfs import SubvolumeSieve
+from btrview.rich_output import logic, SORT_FUNCS
+from btrview.subvolume import SubvolumeSieve
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
@@ -49,15 +49,15 @@
             "--export",
             choices = ("text","svg","html"),
             help = "Export the specifed type instead of a rich table. Using this flag will still write to stdout. If you wish to save to a file use shell redirection.",)
 
     return arg_parser
 
 def main():
-    check_root()
     args = parser().parse_args()
+    check_root()
     output = logic(args.labels, args.exclude, args.property, 
                    args.fold, args.export, SORT_FUNCS[args.sort], not args.ascending)
     print(output)
  
 if __name__ == "__main__":
     main()
```

### Comparing `btrview-0.7.2/btrview/rich_output.py` & `btrview-0.8.0/btrview/rich_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from rich.tree import Tree as RichTree
 from rich.console import Group
 from rich.console import Console
 from rich.table import Table
 from rich.style import Style
 from rich.text import Text
 
-from btrview.btrfs import Btrfs, get_forest, SubvolumeSieve
-from btrview.subvolume import Subvolume
+from btrview.btrfs import get_forest, System
+from btrview.subvolume import Subvolume, SubvolumeSieve
 
 TreeSorter = Callable[[treelib.Tree, treelib.Node], Any]
 
 SORT_FUNCS: dict[str, TreeSorter]= {
         "size": lambda t,n: t.subtree(n.identifier).size(),
         "Creation time": lambda t,n: n.data["Creation time"],
         "Generation": lambda t,n: n.data["Generation"],
@@ -130,15 +130,15 @@
         forest_table.add_column("Snapshot Tree:")
         forest_table.add_row(self.subvol_forest,self.snapshot_forest)
         return forest_table
 
 def logic(labels: list[str], remove: tuple[str,...], prop: str, 
           fold: int, export: str, sort_func:TreeSorter, reverse: bool) -> str:
     """Constructs Rich output based on the parameters given."""
-    filesystems = Btrfs.get_filesystems(labels)
+    filesystems = System.from_fs(labels).filesystems
     tables = []
     for fs in filesystems:
         subvols = fs.subvolumes(remove)
         display = ForestDisplay(subvols)
         subvol_display = display.display_forest("subvol", prop, fold, sort_func, reverse)
         snap_display = display.display_forest("snap", prop, fold, sort_func, reverse)
```

### Comparing `btrview-0.7.2/btrview/scripts/btrview.py` & `btrview-0.8.0/btrview/scripts/btrview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import argparse
 
 import btrview
 from btrview.utils import check_root
-from btrview.rich_output import logic,SORT_FUNCS
-from btrview.btrfs import SubvolumeSieve
+from btrview.rich_output import logic, SORT_FUNCS
+from btrview.subvolume import SubvolumeSieve
 
 def parser() -> argparse.ArgumentParser:
     """Returns the argument parser for the command line arguments"""
     arg_parser = argparse.ArgumentParser(
             description = "Better way to view btrfs filesystems.",
             epilog = f"btrview version {btrview.__version__}, created by Chris Copley")
 
@@ -49,15 +49,15 @@
             "--export",
             choices = ("text","svg","html"),
             help = "Export the specifed type instead of a rich table. Using this flag will still write to stdout. If you wish to save to a file use shell redirection.",)
 
     return arg_parser
 
 def main():
-    check_root()
     args = parser().parse_args()
+    check_root()
     output = logic(args.labels, args.exclude, args.property, 
                    args.fold, args.export, SORT_FUNCS[args.sort], not args.ascending)
     print(output)
  
 if __name__ == "__main__":
     main()
```

### Comparing `btrview-0.7.2/btrview/subvolume.py` & `btrview-0.8.0/btrview/subvolume.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,36 @@
 """Subvolume Classes and errors."""
-from pathlib import Path, PurePath
-from typing import Self
-from dataclasses import dataclass
+from __future__ import annotations
+from pathlib import Path
+from typing import Self, TypeAlias, Callable, Iterable
 
 from btrfsutil import SubvolumeInfo, subvolume_info, subvolume_path
 from btrview.typed_info import BaseInfo, TypedInfo, BTRDICT, BASE
+import btrview.btrfs as btrfs
 
 class NotASubvolumeError(NotADirectoryError):
     """Throw when a directory isn't a subvolume"""
 
-@dataclass(frozen=True)
-class Mount:
-    """Basic class for working with mounted subvolumes."""
-    fsroot: PurePath
-    target: Path
-
-    def resolve(self, path: PurePath) -> Path:
-        """Returns the resolved path of another path"""
-        fsroot_str = str(self.fsroot)
-        target_str = str(self.target)
-        if fsroot_str == "/":
-            target_str = target_str + "/"
-        path_str = str(path)
-        new_path = path_str.replace(fsroot_str,target_str,1).replace("//","/",1)
-        return Path(new_path)
-
-    def __str__(self) -> str:
-        return f"{self.fsroot} on {self.target}"
-
 class Subvolume:
     """Class representing a btrfs subvolume"""
     def __init__(self, 
                  info: BaseInfo, 
-                 mounts: tuple[Mount, ...],
+                 fs: btrfs.Btrfs,
                  deleted = False) -> None:
         self.info = info
-        self.mounts = mounts
+        self.fs = fs
         self.deleted = deleted
 
     @property
     def fs_paths(self) -> list[Path]:
         """Returns all the reachable paths of the Subvolume"""
         if self["Path"] is None:
             return []
         btr_path = self["Path"]
-        paths = [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
+        paths = [mount.resolve(btr_path) for mount in self.fs.mounts if btr_path.is_relative_to(mount.fsroot)]
         paths = [path for path in paths if path.exists()]
         return paths
 
     @property
     def mounted(self) -> bool:
         """Returns whether the subvolume is reachable via the filesystem"""
         return bool(self.fs_paths)
@@ -62,15 +44,15 @@
     def snapshot(self) -> bool:
         """Returns whether the subvolume is a snapshot"""
         return bool(self["Parent UUID"])
 
     @property
     def mount_points(self) -> tuple[Path, ...]:
         """Returns mount points of Subvolume"""
-        targets = [mount.target for mount in self.mounts]
+        targets = [mount.target for mount in self.fs.mounts]
         return tuple(path for path in self.fs_paths if path in targets)
 
     def parent(self, p_type: str) -> str | None:
         """Returns parent UUID or ID string"""
         match p_type:
             case "snap":
                 parent = self["Parent UUID"]
@@ -88,29 +70,29 @@
             case "subvol":
                 ID = self["Subvolume ID"]
             case _:
                 ID = self["UUID"]
         return ID
 
     @classmethod
-    def from_info(cls, path: str, info: SubvolumeInfo, mounts: tuple[Mount, ...]) -> Self:
+    def from_info(cls, path: str, info: SubvolumeInfo, fs: btrfs.Btrfs) -> Self:
         t_info = TypedInfo.from_info(path, info)
-        return cls(t_info, mounts)
+        return cls(t_info, fs)
 
     @classmethod
-    def from_ID(cls, path: str | Path, subvol_id: int, mounts: tuple[Mount, ...]) -> Self:
+    def from_ID(cls, path: str | Path, subvol_id: int, fs: btrfs.Btrfs) -> Self:
         """Creates subvolume from subvolume's ID and any path on the filesystem"""
         info = subvolume_info(path, subvol_id)
         btrfs_path = subvolume_path(path, subvol_id)
-        return cls.from_info(btrfs_path, info, mounts)
+        return cls.from_info(btrfs_path, info, fs)
 
     @classmethod
-    def from_deleted(cls, uuid: str):
+    def from_deleted(cls, uuid: str, fs: btrfs.Btrfs):
         info = TypedInfo.from_deleted(str(uuid))
-        return cls(info, (), True)
+        return cls(info, fs, True)
 
     def __getitem__(self, key: str) -> str | None:
         """Returns the item from TypedInfo object."""
         if key in BTRDICT:
             if not self.deleted:
                 return self.info[key]
             else:
@@ -130,8 +112,41 @@
 
     def __hash__(self) -> int:
         return hash(self["UUID"])
 
     def __eq__(self, other) -> bool:
         return self["UUID"] == other["UUID"]
 
+class SubvolumeSieve:
+    """A class for sieving subvolumes"""
+    SIEVES: dict[str, Sieve] = {
+            "deleted": lambda s: s.deleted,
+            "root": lambda s: s.root_subvolume,
+            "snapshot": lambda s: s.snapshot and not s.root_subvolume,
+            "unreachable": lambda s: not (s.mounted or s.deleted),
+            "non-mounts": lambda s: not s.mount_points
+            }
+
+    def __init__(self, subvolumes: list[Subvolume]) -> None:
+        self.subvolumes = subvolumes
+
+    def sieve_str(self, string_sieves: Iterable[str]):
+        """Removes subvolumes from a list based on string"""
+        sieves = [self.SIEVES[s] for s in string_sieves]
+        return self.sieve(sieves)
+
+    def sieve(self, remove_funcs: Iterable[Sieve]) -> list[Subvolume]:
+        """Remove subvolumes from a list determined by an iterable of sieve functions"""
+        to_remove = []
+        for subvol in self.subvolumes:
+            #if any of them evaluate True, then remove
+            bools = [f(subvol) for f in remove_funcs]
+            remove = any(bools)
+            if remove:
+                #don't want to remove in place while iterating
+                to_remove.append(subvol)
+        copy = self.subvolumes.copy()
+        for subvol in to_remove:
+            copy.remove(subvol)
+        return copy
 
+Sieve: TypeAlias = Callable[[Subvolume], bool]
```

### Comparing `btrview-0.7.2/btrview/typed_info.py` & `btrview-0.8.0/btrview/typed_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes and constants to aid in casting SubvolumeInfo objects."""
+from __future__ import annotations
 from pathlib import PurePath
 from typing import Self
 from datetime import datetime
 from uuid import UUID
 from dataclasses import dataclass
 
 from btrfsutil import SubvolumeInfo
@@ -18,23 +19,22 @@
 
 GENS = {"generation": "Generation",
         "otransid": "Gen at creation",
         "rtransid": "Receive transid",
         "stransid": "Send transid",
         "ctransid": None,}
 
-INTS = {"id": "Subvolume ID",
+NONCAST = {"id": "Subvolume ID",
         "parent_id": "Parent ID",
         "flags": "Flags",
-        "dir_id": None,}
+        "dir_id": None,
+        "name": "Name",
+        "path": "Path",}
 
-OTHER = {"name": "Name",
-         "path": "Path",}
-
-BTRDICT = {v:k for k,v in (UUIDS | TIMES | GENS | INTS | OTHER).items() if v}
+BTRDICT = {v:k for k,v in (UUIDS | TIMES | GENS | NONCAST).items() if v}
 BASE = {k:v for k,v in BTRDICT.items() if v in ("name","id","uuid")}
 
 @dataclass
 class Generation:
     """A class representing a btrfs generation"""
     generation: int
 
@@ -46,15 +46,15 @@
     """Base class for TypedInfo, mainly used to facilitate creating
     subvolume and snapshot trees for subvolumes not on the filesystem"""
     name: str
     id: int
     uuid: UUID
 
     @classmethod
-    def from_deleted(cls, suuid: str) -> "BaseInfo":
+    def from_deleted(cls, suuid: str) -> BaseInfo:
         """Returns a BaseInfo instance from a uuid"""
         uuid = UUID(suuid)
         bi = BaseInfo(suuid, uuid.int, uuid)
         return bi
 
     def __getitem__(self, key: str):
         """Returns the attribute corresponding to the key in BTRDICT"""
@@ -105,11 +105,11 @@
         if key in TIMES:
             return datetime.fromtimestamp(value) if value else None
         elif key in UUIDS:
             value = value.hex()
             return UUID(value) if value != "0"*32 else None
         elif key in GENS:
             return Generation(value) if value else None
-        elif key in INTS:
-            return int(value)
+        elif key in NONCAST:
+            return value
         else:
             raise KeyError(f"{key = } can't be cast")
```

### Comparing `btrview-0.7.2/btrview.egg-info/PKG-INFO` & `btrview-0.8.0/btrview.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.7.2
+Version: 0.8.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,23 +58,31 @@
 Subvolumes that are mounted (in fstab or somehow else) are in bold, those that are grey are subvolumes that aren't currently reachable on the filesystem, and subvolumes in red (not shown here) are not currently on the filesytem. This could be because they're deleted, or maybe its child subvolume was `btrfs received` from another filesystem.
 
 Wondering what the difference between the subvolume and snapshot tree is? [Check out the FAQ](#q-whats-the-difference-between-the-subvolume-tree-and-the-snapshot-tree)!
 
 ## Installation:
 
 Btrview relies on the following dependencies:
-* python 3.11 or greater
-* btrfs-progs
-* python-treelib
-* python-rich
+* [python 3.11 or greater](https://www.python.org/)
+* [findmnt](https://man7.org/linux/man-pages/man8/findmnt.8.html) (should be installed by default on most distributions)
+* [btrfs-progs](https://github.com/kdave/btrfs-progs/tree/master)
+* [python-btrfsutil](https://github.com/kdave/btrfs-progs/tree/master/libbtrfsutil) (might be included with btrfs progs)
+* [python-treelib](https://treelib.readthedocs.io/en/latest/)
+* [python-rich](https://rich.readthedocs.io/en/stable/introduction.html)
 
-The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx install --system-site-packages btrview`. Using pipx to install btrview will also install the required python dependencies and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
+The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx install --system-site-packages btrview`. Using pipx to install btrview will also install treelib and rich and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
 
 If you don't feel like installing via pipx you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
 
+### Installation Troubleshooting
+
+Q: How come when I use the sudo command with btrview I get `sudo: btrview: command not found`, but when I run it without sudo the command is recognized?
+
+A: You are likely are using a linux distribution which hard codes the paths sudo can use to find executables. There are one of two options here, you can either comment out the line that contains "secure_path" in `/etc/sudoers` or you can add the path you're using to that variable. The former option will change it so that any executable in the user's path can be executed, the latter option will merely add the user's path to list of allowed paths.
+
 ## Some Qs and As:
 
 ### Q: What is btrfs?
 
 In short, it's a copy on write (COW) filesystem. If you're not already using btrfs, then check out the [documentation](https://btrfs.readthedocs.io/en/latest/) to see if it's something you'd be interested in.
 
 ### Q: What does btrview do?
```

### Comparing `btrview-0.7.2/pyproject.toml` & `btrview-0.8.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.7.2"
+version = "0.8.0"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 Issues = "https://github.com/CopOnTheRun/btrview/issues"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.7.2"
+current_version = "0.8.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

