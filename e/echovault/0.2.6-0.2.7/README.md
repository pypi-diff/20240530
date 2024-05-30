# Comparing `tmp/echovault-0.2.6.tar.gz` & `tmp/echovault-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echovault-0.2.6.tar", max compression
+gzip compressed data, was "echovault-0.2.7.tar", max compression
```

## Comparing `echovault-0.2.6.tar` & `echovault-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.6/README.md
--rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.6/echovault/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.6/echovault/__init__.py~
--rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.6/echovault/_container.py
--rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.6/echovault/_container.py~
--rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.6/echovault/db.py~
--rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.6/echovault/dict.py
--rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.6/echovault/dict.py~
--rw-r--r--   0        0        0     2366 2024-05-10 17:54:28.098196 echovault-0.2.6/echovault/list.py
--rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.6/echovault/list.py~
--rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.6/echovault/table.py~
--rw-r--r--   0        0        0     7253 2024-05-10 17:53:25.300309 echovault-0.2.6/echovault/vault.py
--rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.6/echovault/vault.py.bck
--rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.6/echovault/vault.py~
--rw-r--r--   0        0        0      380 2024-05-10 17:57:41.072393 echovault-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.7/README.md
+-rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.7/echovault/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.7/echovault/__init__.py~
+-rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.7/echovault/_container.py
+-rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.7/echovault/_container.py~
+-rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.7/echovault/db.py~
+-rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.7/echovault/dict.py
+-rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.7/echovault/dict.py~
+-rw-r--r--   0        0        0     2366 2024-05-10 17:54:28.098196 echovault-0.2.7/echovault/list.py
+-rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.7/echovault/list.py~
+-rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.7/echovault/table.py~
+-rw-r--r--   0        0        0     8975 2024-05-29 19:57:42.004984 echovault-0.2.7/echovault/vault.py
+-rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.7/echovault/vault.py.bck
+-rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.7/echovault/vault.py~
+-rw-r--r--   0        0        0      380 2024-05-30 14:07:20.120861 echovault-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.7/PKG-INFO
```

### Comparing `echovault-0.2.6/README.md` & `echovault-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/_container.py` & `echovault-0.2.7/echovault/_container.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/_container.py~` & `echovault-0.2.7/echovault/_container.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/dict.py` & `echovault-0.2.7/echovault/dict.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/dict.py~` & `echovault-0.2.7/echovault/dict.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/list.py` & `echovault-0.2.7/echovault/list.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/list.py~` & `echovault-0.2.7/echovault/list.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/table.py~` & `echovault-0.2.7/echovault/table.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/echovault/vault.py` & `echovault-0.2.7/echovault/vault.py.bck`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 except:
     def getuid():
         return None
 
     def getgid():
         return None
 
-ref_head = b'refs/heads/'
-    
 def walk_ancestor(object_store, commit):
     for identifier in commit.parents:
         yield identifier
 
     for identifier in commit.parents:
         yield from walk(object_store, object_store[identifier])
     
@@ -49,49 +47,43 @@
     
     return common_ancestor
 
 class Conflict(Exception):
     pass
 
 class Vault(Container):
-    List = List
-    
     @staticmethod
     def encode(string):
         return string.encode('utf-8')
 
     @staticmethod
     def decode(value):
         return value.decode('utf-8')
     
     def __init__(self, object_store, refs, *, tree:Tree=None, ref=None):
         super().__init__(object_store, None, None, tree)
         self.refs = refs
         if ref is not None:
             self.checkout(ref)
         else:
-            self._ref = None
+            self.ref = None
 
-    @property
-    def ref(self):
-        return self._ref[len(ref_head):].decode('utf-8')
-            
     def __getitem__(self, name:str):
         identifier = self.encode(name)
         _, oid = self.tree[identifier]
         tree = self.object_store[oid]
-        return self.List(self.object_store,
-                         self,
-                         identifier,
-                         tree=tree)
+        return List(self.object_store,
+                     self,
+                     identifier,
+                     tree=tree)
 
     def __setitem__(self, name:str, iterable):
         identifier = self.encode(name)
         self.tree[identifier] = S_IFDIR, None
-        table = self.List(self.object_store, self, identifier, iterable)
+        table = List(self.object_store, self, identifier, iterable)
         self._update()
 
     def __delitem__(self, name:str):
         del self.tree[self.encode(name)]
         self._update()
 
     def __iter__(self):
@@ -113,47 +105,43 @@
 
     def __repr__(self):
         return repr({key: value
                      for key, value
                      in self.items()})
             
     def rollback(self):
-        if self._ref is None:
+        if self.ref is None:
             self.tree = Tree()
         else:
             self.tree = self.object_store[self.object_store[self.refs[ref]].tree]
 
-    def checkout(self, ref, branch=False):
-        tree = self.tree
+    def checkout(self, ref):
+        tree = Tree()
         
-        ref = ref_head + ref.encode('utf-8')
+        ref = b'refs/heads/' + ref.encode('utf-8')
         
         if ref in self.refs:
             tree = self.object_store[self.object_store[self.refs[ref]].tree]
-        elif branch:
-            self.refs[ref] = self.refs[self._ref]
-        else:
-            raise ValueError(f"No {ref} branch is existing !")
-            
-        self._ref = ref
+        
+        self.ref = ref
         self.tree = tree
         
             
     def commit(self,
                ref:Optional[str]=None,
                message:Optional[str]='',
                author:Optional[str]=None,
                committer:Optional[str]=None,
                time_:Optional[int]=None,
                timezone:Optional[int]=None,
                ):
         if ref is None:
-            ref = self._ref
+            ref = self.ref
         else:
-            ref = ref_head + ref.encode('utf-8')
+            ref = b'refs/heads/' + ref.encode('utf-8')
             
         commit = Commit()
         
         commit.message = message.encode('utf-8')
         commit.tree = self.tree
 
         if committer is None:
@@ -180,16 +168,16 @@
         commit.commit_time = time_
         commit.commit_timezone = timezone
         commit.author_time = time_
         commit.author_timezone = timezone
 
         if ref in self.refs:
             parents = (self.refs[ref],)
-        elif self._ref in self.refs:
-            parents = (self.refs[self._ref],)
+        elif self.ref in self.refs:
+            parents = (self.refs[self.ref],)
         else:
             parents = ()
             
         commit.parents = parents
         
         if not commit.id in self.object_store:
             self.object_store.add_object(commit)
@@ -230,14 +218,38 @@
                         self[key] = entries
                 case ('!=', name, *difference):
                     self[name].patch((difference,))
 
     def merge(self, others, *, without_conflict=True):
         ancestor = last_common_ancestor(self.object_store,
                                         self.refs,
-                                        (vault._ref for vault in (self, *others)))
+                                        (vault.ref for vault in (self, *others)))
 
         base_vault = Vault(self.object_store, self.refs,
                            tree=self.object_store[self.object_store[ancestor].tree])
 
+        applied_differences = {}
+        for difference inself.diff(base_vault):
+            match difference:
+                case ('-', removed):
+                    
+        
         for child in others:
-            self.patch(child.diff(base_vault))
+            
+            for difference in base:
+                conflict = set()
+                match difference:
+                    case ('-', removed):
+                        conflict = removed.intersection(applied_differences[None]['+'])
+                    case ('+', added):
+                        conflict = added.intersection(applied_differences[None]['-'])
+                    case ('!=', table, '-', removed):
+                        conflict = removed.intersection(applied_differences[table]['+'])
+                    case ('!=', table, '+', added):
+                        conflict = added.intersection(applied_differences[table]['-'])
+                    case ('!=', table, '!=', entry, '-', keys):
+                        conflict = added.intersection(applied_differences[table][entry][])
+
+                if conflict:
+                    raise Conflict(f'operation {difference} about {conflict} made on {child} conflicts with other merged vaults.')
+                
+                self.patch((difference,))
```

### Comparing `echovault-0.2.6/echovault/vault.py.bck` & `echovault-0.2.7/echovault/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from dulwich.objects import Tree, Commit
+from dulwich.repo import Repo
+from dulwich.client import get_transport_and_path
+from dulwich.protocol import ZERO_SHA
 from echovault.list import List
 from base64 import b64decode, b64encode
 from socket import getfqdn, gethostname
+from datetime import datetime
 from os import getpid, getlogin, name as operating_system_name
 from sys import argv
 from typing import Optional
 from time import time
 from stat import S_IFDIR
 from echovault._container import Container
 
@@ -14,14 +18,16 @@
 except:
     def getuid():
         return None
 
     def getgid():
         return None
 
+ref_head = b'refs/heads/'
+
 def walk_ancestor(object_store, commit):
     for identifier in commit.parents:
         yield identifier
 
     for identifier in commit.parents:
         yield from walk(object_store, object_store[identifier])
     
@@ -47,43 +53,49 @@
     
     return common_ancestor
 
 class Conflict(Exception):
     pass
 
 class Vault(Container):
+    List = List
+    
     @staticmethod
     def encode(string):
         return string.encode('utf-8')
 
     @staticmethod
     def decode(value):
         return value.decode('utf-8')
     
     def __init__(self, object_store, refs, *, tree:Tree=None, ref=None):
         super().__init__(object_store, None, None, tree)
         self.refs = refs
         if ref is not None:
             self.checkout(ref)
         else:
-            self.ref = None
+            self._ref = None
 
+    @property
+    def ref(self):
+        return self._ref[len(ref_head):].decode('utf-8')
+            
     def __getitem__(self, name:str):
         identifier = self.encode(name)
         _, oid = self.tree[identifier]
         tree = self.object_store[oid]
-        return List(self.object_store,
-                     self,
-                     identifier,
-                     tree=tree)
+        return self.List(self.object_store,
+                         self,
+                         identifier,
+                         tree=tree)
 
     def __setitem__(self, name:str, iterable):
         identifier = self.encode(name)
         self.tree[identifier] = S_IFDIR, None
-        table = List(self.object_store, self, identifier, iterable)
+        table = self.List(self.object_store, self, identifier, iterable)
         self._update()
 
     def __delitem__(self, name:str):
         del self.tree[self.encode(name)]
         self._update()
 
     def __iter__(self):
@@ -105,59 +117,96 @@
 
     def __repr__(self):
         return repr({key: value
                      for key, value
                      in self.items()})
             
     def rollback(self):
-        if self.ref is None:
+        if self._ref is None:
             self.tree = Tree()
         else:
             self.tree = self.object_store[self.object_store[self.refs[ref]].tree]
 
-    def checkout(self, ref):
-        tree = Tree()
+    def checkout(self, ref, branch=False):
+        tree = self.tree
         
-        ref = b'refs/heads/' + ref.encode('utf-8')
+        ref = ref_head + ref.encode('utf-8')
         
         if ref in self.refs:
             tree = self.object_store[self.object_store[self.refs[ref]].tree]
-        
-        self.ref = ref
+        elif branch:
+            self.refs[ref] = self.refs[self._ref]
+        else:
+            raise ValueError(f"No {ref} branch is existing !")
+            
+        self._ref = ref
         self.tree = tree
+
+    def fetch(self, remote_uri, ref:Optional[str]=None):
+        destination = Repo(self.refs.path.decode('utf-8'), bare=True)
+        # TODO: implement determine_wants function based on ref (or self._ref ?)
+        client, source = get_transport_and_path(remote_uri)
         
-            
+        def determine_wants(refs, depth=None):
+            wanted_tips = list(refs.values())
+            return wanted_tips
+
+        # instead of changing local head branch we shall have update "remotes/{branch_name}"
+        client.fetch(source, destination, determine_wants)
+
+    def pull(self, remote_uri, ref:Optional[str]=None):
+        self.fetch(remote_uri, ref)
+        self.patch(self.diff(Vault(self.object_store, self.refs,
+                                   ref=(ref.encode('utf-8')
+                                        if ref is not None
+                                        else self.ref))))
+        
+    def push(self, remote_uri, ref:Optional[str]=None):
+        source = Repo(self.refs.path.decode('utf-8'), bare=True)
+        client, destination = get_transport_and_path(remote_uri)
+
+        def update_refs(refs):
+            # TODO: reduce dictionaire to ref (or self._ref ?)
+            return {ref: (self.refs[ref]
+                          if ref in self.refs
+                          else ZERO_SHA)
+                    for ref
+                    in set(refs).union(set(self.refs.keys()))
+                    if ref.startswith(b'refs/heads/')}
+
+        client.send_pack(destination,
+                         update_refs,
+                         source.generate_pack_data)
+
     def commit(self,
                ref:Optional[str]=None,
                message:Optional[str]='',
                author:Optional[str]=None,
                committer:Optional[str]=None,
                time_:Optional[int]=None,
                timezone:Optional[int]=None,
                ):
         if ref is None:
-            ref = self.ref
+            ref = self._ref
         else:
-            ref = b'refs/heads/' + ref.encode('utf-8')
+            ref = ref_head + ref.encode('utf-8')
             
         commit = Commit()
         
-        commit.message = message.encode('utf-8')
         commit.tree = self.tree
 
         if committer is None:
             committer = ('_'.join((getfqdn(), gethostname(),
                                    operating_system_name,
                                    repr(getgid()),
                                    repr(getuid()), repr(getpid())))
-                         + ': '
-                         + ' '.join(argv))
+                         + f' <{getlogin()}@{getfqdn()}>')
             
         if author is None:
-            author = getlogin()
+            author = f'{getlogin()} <{getlogin()}@{getfqdn()}>'
 
             
         commit.committer = committer.encode('utf-8')
         commit.author = author.encode('utf-8')
 
         if time_ is None:
             time_ = int(time())
@@ -168,21 +217,23 @@
         commit.commit_time = time_
         commit.commit_timezone = timezone
         commit.author_time = time_
         commit.author_timezone = timezone
 
         if ref in self.refs:
             parents = (self.refs[ref],)
-        elif self.ref in self.refs:
-            parents = (self.refs[self.ref],)
+        elif self._ref in self.refs:
+            parents = (self.refs[self._ref],)
         else:
             parents = ()
             
         commit.parents = parents
         
+        commit.message = message.encode('utf-8')
+
         if not commit.id in self.object_store:
             self.object_store.add_object(commit)
 
         self.refs[ref] = commit.id
 
     def diff(self, other):
         if self.tree.id == other.tree.id:
@@ -218,38 +269,14 @@
                         self[key] = entries
                 case ('!=', name, *difference):
                     self[name].patch((difference,))
 
     def merge(self, others, *, without_conflict=True):
         ancestor = last_common_ancestor(self.object_store,
                                         self.refs,
-                                        (vault.ref for vault in (self, *others)))
+                                        (vault._ref for vault in (self, *others)))
 
         base_vault = Vault(self.object_store, self.refs,
                            tree=self.object_store[self.object_store[ancestor].tree])
 
-        applied_differences = {}
-        for difference inself.diff(base_vault):
-            match difference:
-                case ('-', removed):
-                    
-        
         for child in others:
-            
-            for difference in base:
-                conflict = set()
-                match difference:
-                    case ('-', removed):
-                        conflict = removed.intersection(applied_differences[None]['+'])
-                    case ('+', added):
-                        conflict = added.intersection(applied_differences[None]['-'])
-                    case ('!=', table, '-', removed):
-                        conflict = removed.intersection(applied_differences[table]['+'])
-                    case ('!=', table, '+', added):
-                        conflict = added.intersection(applied_differences[table]['-'])
-                    case ('!=', table, '!=', entry, '-', keys):
-                        conflict = added.intersection(applied_differences[table][entry][])
-
-                if conflict:
-                    raise Conflict(f'operation {difference} about {conflict} made on {child} conflicts with other merged vaults.')
-                
-                self.patch((difference,))
+            self.patch(child.diff(base_vault))
```

### Comparing `echovault-0.2.6/echovault/vault.py~` & `echovault-0.2.7/echovault/vault.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.6/PKG-INFO` & `echovault-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echovault
-Version: 0.2.6
+Version: 0.2.7
 Summary: echovault is git data storage
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

