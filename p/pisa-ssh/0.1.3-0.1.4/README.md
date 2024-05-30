# Comparing `tmp/pisa_ssh-0.1.3.tar.gz` & `tmp/pisa_ssh-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisa_ssh-0.1.3.tar", last modified: Sat May 11 15:43:32 2024, max compression
+gzip compressed data, was "pisa_ssh-0.1.4.tar", last modified: Thu May 30 15:00:36 2024, max compression
```

## Comparing `pisa_ssh-0.1.3.tar` & `pisa_ssh-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.775174 pisa_ssh-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/dispatcher/cluster_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/dispatcher/task_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-11 15:43:17.000000 pisa_ssh-0.1.3/src/pisa/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:43:32.779174 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 15:43:32.000000 pisa_ssh-0.1.3/src/pisa_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:00:36.683312 pisa_ssh-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-30 15:00:36.683312 pisa_ssh-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:00:36.683312 pisa_ssh-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:00:36.679312 pisa_ssh-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:00:36.679312 pisa_ssh-0.1.4/src/pisa/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:00:36.679312 pisa_ssh-0.1.4/src/pisa/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/dispatcher/cluster_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/dispatcher/task_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:00:36.679312 pisa_ssh-0.1.4/src/pisa/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-30 15:00:18.000000 pisa_ssh-0.1.4/src/pisa/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:00:36.683312 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-30 15:00:36.000000 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-30 15:00:36.000000 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:00:36.000000 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 15:00:36.000000 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 15:00:36.000000 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 15:00:36.000000 pisa_ssh-0.1.4/src/pisa_ssh.egg-info/top_level.txt
```

### Comparing `pisa_ssh-0.1.3/LICENSE` & `pisa_ssh-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.3/PKG-INFO` & `pisa_ssh-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pisa_ssh-0.1.3/README.md` & `pisa_ssh-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.3/pyproject.toml` & `pisa_ssh-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.3/src/pisa/__main__.py` & `pisa_ssh-0.1.4/src/pisa/__main__.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.3/src/pisa/dispatcher/cluster_conf.py` & `pisa_ssh-0.1.4/src/pisa/dispatcher/cluster_conf.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.3/src/pisa/dispatcher/dispatcher.py` & `pisa_ssh-0.1.4/src/pisa/dispatcher/dispatcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,22 +26,21 @@
     while True:
         try:
             # get a task from the queue
             task = tasks.get(block=False)
             has_task = True
             log.debug(f"Task {task.num} starting on node {node.get_address()}: {task.cmd}")
 
-            ssh.Session(node.get_address()) \
-                .connect() \
-                .send_command(f"cd {task.w_dir}") \
-                .send_command(f"./{task.env}/bin/activate") \
-                .send_command(f"mkdir -p {task.out}") \
-                .send_command(f"mkdir -p {task.err}") \
-                .send_command(f"nice -n 19 {task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err") \
-                .close()
+            ssh.Session(node.get_address()).connect().send_command_list([
+                f"cd {task.w_dir}",
+                f"./{task.env}/bin/activate",
+                f"mkdir -p {task.out}",
+                f"mkdir -p {task.err}",
+                f"nice -n 19 {task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err"
+            ]).close()
             # log.debug(f"{task.cmd} >{task.out}/{task.num}.out 2>{task.err}/{task.num}.err &")  # TODO: remove
         except queue.Empty:  # queue is empty: exit thread
             has_task = False
             break
         except FileNotFoundError as e:  # file not found: program is not available
             log.error(f"file not found: {e}")
             tasks.put(task)  # reinsert task back into the queue
```

### Comparing `pisa_ssh-0.1.3/src/pisa/dispatcher/task_list.py` & `pisa_ssh-0.1.4/src/pisa/dispatcher/task_list.py`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.1.3/src/pisa/ssh/ssh.py` & `pisa_ssh-0.1.4/src/pisa/ssh/ssh.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,31 +30,39 @@
 
     def send_command(self, command):
         self._check_connected()
         self.ssh_process.stdin.write(f"{command}\n".encode('utf-8'))
         self.ssh_process.stdin.flush()
         return self  # monadic return
 
+    def send_command_list(self, cmd_list: list):
+        self._check_connected()
+        for command in cmd_list:
+            self.send_command(command)
+            # self.ssh_process.stdin.write(f"{command}\n".encode('utf-8'))
+            # self.ssh_process.stdin.flush()
+        return self  # monadic return
+
     def read_stdout(self):
         self._check_connected()
         return self.ssh_process.stdout.read1().decode('utf-8')
 
     def read_stderr(self):
         self._check_connected()
         return self.ssh_process.stderr.read1().decode('utf-8')
 
-    def wait(self):
+    def wait_for_exit(self):
         self._check_connected()
         self.ssh_process.wait()
         return self  # monadic return
 
     def close(self):
         if self.ssh_process is not None:
             self.ssh_process.stdin.write("exit\n".encode('utf-8'))
             try:
                 self.ssh_process.stdin.flush()
             except BrokenPipeError:
                 pass
-            self.wait()
+            self.wait_for_exit()
 
     def __del__(self):
         self.close()
```

### Comparing `pisa_ssh-0.1.3/src/pisa_ssh.egg-info/PKG-INFO` & `pisa_ssh-0.1.4/src/pisa_ssh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
```

