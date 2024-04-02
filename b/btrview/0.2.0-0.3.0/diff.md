# Comparing `tmp/btrview-0.2.0.tar.gz` & `tmp/btrview-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.2.0.tar", last modified: Tue Mar 12 16:37:37 2024, max compression
+gzip compressed data, was "btrview-0.3.0.tar", last modified: Tue Apr  2 00:14:34 2024, max compression
```

## Comparing `btrview-0.2.0.tar` & `btrview-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-03-12 16:37:37.983622 btrview-0.2.0/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.2.0/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     5356 2024-03-12 16:37:37.983622 btrview-0.2.0/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     3731 2024-03-12 16:26:42.000000 btrview-0.2.0/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-03-12 16:37:37.980289 btrview-0.2.0/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       66 2024-03-12 16:37:17.000000 btrview-0.2.0/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1649 2024-03-12 00:21:46.000000 btrview-0.2.0/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6236 2024-03-12 13:35:58.000000 btrview-0.2.0/btrview/mounts.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-03-12 16:37:37.983622 btrview-0.2.0/btrview/scripts/
--rwxr--r--   0 chris     (1000) chris     (1000)     1660 2024-02-23 19:49:13.000000 btrview-0.2.0/btrview/scripts/btrsend.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     1649 2024-03-12 00:21:46.000000 btrview-0.2.0/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5219 2024-03-12 13:37:58.000000 btrview-0.2.0/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-02-27 20:37:50.000000 btrview-0.2.0/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-03-12 16:37:37.983622 btrview-0.2.0/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     5356 2024-03-12 16:37:37.000000 btrview-0.2.0/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      373 2024-03-12 16:37:37.000000 btrview-0.2.0/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-03-12 16:37:37.000000 btrview-0.2.0/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-03-12 16:37:37.000000 btrview-0.2.0/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-03-12 16:37:37.000000 btrview-0.2.0/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-03-12 16:37:37.000000 btrview-0.2.0/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)      923 2024-03-12 16:37:17.000000 btrview-0.2.0/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-03-12 16:37:37.983622 btrview-0.2.0/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.899686 btrview-0.3.0/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2023-05-17 21:10:51.000000 btrview-0.3.0/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-02 00:14:34.896350 btrview-0.3.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     5932 2024-04-01 23:56:02.000000 btrview-0.3.0/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.896350 btrview-0.3.0/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       65 2024-04-02 00:03:20.000000 btrview-0.3.0/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2372 2024-04-01 23:05:07.000000 btrview-0.3.0/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6215 2024-04-01 23:13:39.000000 btrview-0.3.0/btrview/btrfs.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.896350 btrview-0.3.0/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     1660 2024-03-12 18:06:35.000000 btrview-0.3.0/btrview/scripts/btrsend.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2372 2024-04-01 23:05:07.000000 btrview-0.3.0/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6827 2024-04-01 23:05:07.000000 btrview-0.3.0/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-03-21 15:13:50.000000 btrview-0.3.0/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-04-02 00:14:34.896350 btrview-0.3.0/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     7557 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      372 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-04-02 00:14:34.000000 btrview-0.3.0/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)      923 2024-04-02 00:03:20.000000 btrview-0.3.0/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-04-02 00:14:34.899686 btrview-0.3.0/setup.cfg
```

### Comparing `btrview-0.2.0/LICENSE.md` & `btrview-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.2.0/btrview/mounts.py` & `btrview-0.3.0/btrview/btrfs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,32 @@
 """Classes and functions to interact with a btrfs filesystem."""
 import json
 import re
 from collections import defaultdict
 from pathlib import Path, PurePath
 from typing import Self
-from dataclasses import dataclass
 
 from treelib import Tree
 
 from btrview.utils import run
-from btrview.subvolume import Subvolume
-
-@dataclass(frozen=True)
-class Mount:
-    """Basic class for working with mounted subvolumes."""
-    fsroot: PurePath
-    target: Path
-
-    def resolve(self, path: str) -> Path:
-        """Returns the resolved path of another path"""
-        fsroot_str = str(self.fsroot)
-        target_str = str(self.target)
-        path_str = str(path)
-        new_path = path_str.replace(fsroot_str,target_str,1).replace("//","/",1)
-        return Path(new_path)
-
-    def __str__(self):
-        return f"{self.fsroot} on {self.target}"
+from btrview.subvolume import Subvolume, Mount
 
 class Btrfs:
     """A class representing a btrfs filesystem"""
     _UUIDs:  dict[str,str] = dict()
     _all_mounts: defaultdict[str,set[Mount]] = defaultdict(set)
 
-    def __init__(self, uuid: str, label: str|None = None):
+    def __init__(self, uuid: str, label: str|None = None) -> None:
         """Initialist with the filesystem uuid, and label if it exists."""
         self.uuid = uuid
         self.label = label
         self._get_mounts()
 
     @classmethod
-    def _get_mounts(cls):
+    def _get_mounts(cls) -> None:
         """Generates all the mount points for each filesystem"""
         headings = "label,uuid,fsroot,target"
         #Why parse all mounts instead of just one using the --source flag?
         #Some of the FSes weren't showing up for some reason with that flag. Also
         #it would mean running the command for every FS. Unfortunately if this 
         #method isn't run, then self.mounts will incorrectly return an empty list.
         cmd = f"findmnt --list --json --types btrfs --output {headings}"
@@ -78,54 +60,63 @@
         """Returns a list of deleted subvolumes"""
         uuids = {s["UUID"] for s in subvols}
         puuids = set()
         for subvol in subvols:
             puuid = subvol["Parent UUID"]
             if puuid and (puuid not in uuids):
                 puuids.add(puuid)
-        return [Subvolume({"UUID":puuid}, deleted=True) for puuid in puuids]
+        return [Subvolume({"UUID":puuid}, tuple(), deleted=True) for puuid in puuids]
             
-    def subvolumes(self, root: bool, deleted: bool) -> list[Subvolume]:
+    def subvolumes(self, root: bool, deleted: bool, unreachable: bool,) -> list[Subvolume]:
         """Return a list of subvolumes on the file system"""
         mount_point = self.mounts[0].target 
         out = run(f"btrfs subvolume list -u {mount_point}")
         fs_uuids = []
         subvols = []
         for line in out.stdout.splitlines():
             match = re.search(r"uuid\s*(\S*)",line)
             if match:
                 fs_uuids.append(match.group(1))
         for uuid in fs_uuids:
-            subvol = Subvolume.from_UUID(uuid,mount_point)
+            subvol = Subvolume.from_UUID(uuid, mount_point, self.mounts)
             subvols.append(subvol)
+        if not unreachable:
+            to_remove = []
+            for subvol in subvols:
+                if not subvol.mounted:
+                    to_remove.append(subvol)
+            for subvol in to_remove:
+                subvols.remove(subvol)
+        #order matters here, root should override unreachable
         if root:
-            root_subvol = Subvolume.from_ID("5",mount_point)
+            root_subvol = Subvolume.from_ID("5", mount_point, self.mounts)
             subvols.append(root_subvol)
+        #but also deleted needs to go after root
+        #this is kinda fragile, plan to fix it soon™
         if deleted:
             subvols.extend(self._get_deleted_subvols(subvols))
         return subvols
 
-    def forest(self, snapshots = False, root = True, deleted = False) -> list[Tree]:
+    def forest(self, snapshots = False, root = True, deleted = False, unreachable = True,) -> list[Tree]:
         """Returns a forest of subvolumes with parent/child relationships
         being based on subvolume layout or snapshots."""
         kind = "snap" if snapshots else "subvol"
-        return get_forest(self.subvolumes(root, deleted), kind)
+        if kind == "subvol":
+            deleted = False
+        return get_forest(self.subvolumes(root, deleted, unreachable), kind)
         
     def __str__(self) -> str:
         label =  f"Label: {self.label}"
         uuid = f"UUID: {self.uuid}"
         return f"{label}\n{uuid}"
 
 def subvol_in_list(ID: str, subvolumes: list[Subvolume], kind = "subvol") -> Subvolume | None:
     """Returns a subvolume from a list if there, else returns None."""
-    key = "Subvolume ID"
-    if kind == "snap":
-        key = "UUID"
     for subvolume in subvolumes:
-        if subvolume[key] == ID:
+        if subvolume.id(kind) == ID:
             return subvolume
     return None
 
 def subvol_in_forest(ID: str, trees:list[Tree]) -> Tree | None:
     """Returns the tree containing the specified ID if there, else returns None"""
     for tree in trees:
         if ID in tree:
@@ -146,14 +137,14 @@
         tree.create_node(name, subvol_id, parent_id, data=subvol)
     else:
         tree = Tree()
         trees.append(tree)
         tree.create_node(name, subvol_id, data=subvol)
     return tree
 
-def get_forest(subvolumes: list[Subvolume], kind = "subvol"):
+def get_forest(subvolumes: list[Subvolume], kind = "subvol") -> list[Tree]:
     """Turns a flat list of subvolumes into a forest of trees."""
     trees: list[Tree] = []
     while subvolumes:
         subvol = subvolumes[0]
         get_tree(subvol, subvolumes, trees, kind)
     return trees
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `btrview-0.2.0/btrview/scripts/btrsend.py` & `btrview-0.3.0/btrview/scripts/btrsend.py`

 * *Files identical despite different names*

### Comparing `btrview-0.2.0/btrview/subvolume.py` & `btrview-0.3.0/btrview/subvolume.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,63 @@
 """Subvolume Classes and errors."""
 import subprocess
 import re
-from pathlib import Path
+from pathlib import Path, PurePath
 from datetime import datetime
 from typing import Self
+from dataclasses import dataclass
 
 from btrview.utils import get_UUIDs, run
 
 class NotASubvolumeError(NotADirectoryError):
     """Throw when a directory isn't a subvolume"""
 
+@dataclass(frozen=True)
+class Mount:
+    """Basic class for working with mounted subvolumes."""
+    fsroot: PurePath
+    target: Path
+
+    def resolve(self, path: str) -> Path:
+        """Returns the resolved path of another path"""
+        fsroot_str = str(self.fsroot)
+        target_str = str(self.target)
+        if fsroot_str == "/":
+            target_str = target_str + "/"
+        path_str = str(path)
+        new_path = path_str.replace(fsroot_str,target_str,1).replace("//","/",1)
+        return Path(new_path)
+
+    def __str__(self) -> str:
+        return f"{self.fsroot} on {self.target}"
+
 class Subvolume:
     """Class representing a btrfs subvolume"""
-    def __init__(self, props: dict[str,str|None], deleted: bool = False) -> None:
+    def __init__(self, props: dict[str,str|None], mounts: tuple[Mount, ...],
+                 deleted: bool = False,) -> None:
         self.props = props
+        self.mounts = mounts
         self.deleted = deleted
 
+    @property
+    def paths(self) -> list[Path]:
+        if not self["btrfs Path"]:
+            return []
+        btr_path = Path(self["btrfs Path"])
+        return [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
+
+    @property
+    def mounted(self) -> bool:
+        return bool(self.paths)
+
+    @property
+    def mount_points(self) -> tuple[Path, ...]:
+        targets = [mount.target for mount in self.mounts]
+        return tuple(path for path in self.paths if path in targets)
+
     def parent(self, p_type: str) -> str | None:
         """Returns parent UUID or ID string"""
         match p_type:
             case "snap":
                 parent = self["Recieved UUID"] or self["Parent UUID"]
             case "subvol":
                 parent = self["Parent ID"]
@@ -35,26 +73,26 @@
             case "subvol":
                 ID = self["Subvolume ID"]
             case _:
                 ID = None
         return ID
 
     @classmethod
-    def from_UUID(cls, uuid: str, path: str | Path) -> Self:
+    def from_UUID(cls, uuid: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from the subvolumes UUID and any path on the filesystem"""
         cmd = f"btrfs subvolume show -u {uuid} {path}"
         props = cls._run_cmd(cmd)
-        return cls(props)
+        return cls(props, mounts)
 
     @classmethod
-    def from_ID(cls, ID: str, path: str | Path) -> Self:
+    def from_ID(cls, ID: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from subvolume's ID and any path on the filesystem"""
         cmd = f"btrfs subvolume show -r {ID} {path}"
         props = cls._run_cmd(cmd)
-        return cls(props)
+        return cls(props, mounts)
 
     @classmethod
     def _run_cmd(cls, cmd: str) -> dict[str, str | None]:
         """Runs the shell command and returns the prop dictionary
         if the command doesn't error"""
         out = run(cmd)
         if out.returncode != 0:
@@ -63,15 +101,17 @@
         return props
 
     @classmethod
     def _get_props(cls, btrfs_show_text: str) -> dict[str, str | None]:
         """Creates btrfs prop dict based on the output of 
         btrfs subvolume show."""
         subvol = {}
-        for line in btrfs_show_text.splitlines():
+        lines = btrfs_show_text.splitlines()
+        subvol["btrfs Path"] = ("/" + lines[0]).replace("//","/")
+        for line in lines[1:]:
             if re.search(r":\s+",line):
                 k,v = line.split(":",maxsplit=1)
                 k = k.strip()
                 v = v.strip()
                 v = None if v == "-" else v
                 subvol[k] = v
         return subvol
@@ -84,26 +124,30 @@
 
     def __getitem__(self, key: str) -> str | None:
         """Returns the item from the props dictionary, but instead
         of throwing a key error, returns None"""
         return self.props.get(key)
 
     def __str__(self) -> str:
-        return self["Name"] or str(self["UUID"])
+        string = self["Name"] or str(self["UUID"])
+        if mps := self.mount_points:
+            mp_string = ", ".join(str(mp) for mp in mps)
+            string = f"{string} on: {mp_string}"
+        return string
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self["UUID"])
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self["UUID"] == other["UUID"]
 
 class MountedSubvolume(Subvolume):
     """Class representing a mounted subvolume. Differs from a normal Subvolume
     in that it can be snapshotted and sent since there's a path to it."""
-    def __init__(self, props: dict[str, str| None], path: Path):
+    def __init__(self, props: dict[str, str| None], path: Path) -> None:
         self.props = props
         self.path = path
 
     @classmethod
     def from_path(cls, path: str | Path) -> Self:
         cmd = f"btrfs subvolume show {path}"
         props = cls._run_cmd(cmd)
@@ -138,9 +182,9 @@
             print(e)
         return type(self).from_path(path / self.path.name)
 
     def delete(self) -> Subvolume:
         """Deletes the subvolume"""
         run(f"btrfs subvolume delete '{self}'")
         props = {"UUID":self["UUID"]}
-        return Subvolume(props,deleted=True)
+        return Subvolume(props, tuple(), deleted=True)
```

### Comparing `btrview-0.2.0/btrview/utils.py` & `btrview-0.3.0/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.2.0/pyproject.toml` & `btrview-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.2.0"
+version = "0.3.0"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,15 +20,15 @@
 btrview = "btrview.scripts.btrview:main"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

