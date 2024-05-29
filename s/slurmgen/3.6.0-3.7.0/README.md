# Comparing `tmp/slurmgen-3.6.0.tar.gz` & `tmp/slurmgen-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmgen-3.6.0.tar", last modified: Fri May 24 15:01:36 2024, max compression
+gzip compressed data, was "slurmgen-3.7.0.tar", last modified: Wed May 29 23:48:22 2024, max compression
```

## Comparing `slurmgen-3.6.0.tar` & `slurmgen-3.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.063351 slurmgen-3.6.0/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.6.0/.gitignore
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.6.0/LICENSE.txt
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-24 15:01:36.063351 slurmgen-3.6.0/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.6.0/README.md
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.059351 slurmgen-3.6.0/example/
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.059351 slurmgen-3.6.0/example/data_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/data_output/goodbye.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/data_output/hello.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 21:53:10.000000 slurmgen-3.6.0/example/job_def.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 21:27:31.000000 slurmgen-3.6.0/example/job_tmpl.json
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1063 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/run_slurm.py
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.059351 slurmgen-3.6.0/example/slurm_output/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      782 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/slurm_output/test.log
--rwxrw-r--   0 tguillod  (1000) tguillod  (1000)     1271 2024-05-24 14:52:38.000000 slurmgen-3.6.0/example/slurm_output/test.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.6.0/pyproject.toml
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.6.0/run_release.sh
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-24 15:01:36.063351 slurmgen-3.6.0/setup.cfg
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.063351 slurmgen-3.6.0/slurmgen/
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-24 14:43:56.000000 slurmgen-3.6.0/slurmgen/__init__.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7930 2024-05-24 14:52:38.000000 slurmgen-3.6.0/slurmgen/gen.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     3249 2024-05-24 14:52:38.000000 slurmgen-3.6.0/slurmgen/run.py
--rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7461 2024-05-24 14:52:38.000000 slurmgen-3.6.0/slurmgen/script.py
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-24 15:01:35.000000 slurmgen-3.6.0/slurmgen/version.txt
-drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-24 15:01:36.063351 slurmgen-3.6.0/slurmgen.egg-info/
--rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/PKG-INFO
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      503 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/SOURCES.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/dependency_links.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/entry_points.txt
--rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-24 15:01:36.000000 slurmgen-3.6.0/slurmgen.egg-info/top_level.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-29 23:48:22.257088 slurmgen-3.7.0/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      278 2023-11-27 16:21:41.000000 slurmgen-3.7.0/.gitignore
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1303 2023-11-27 14:39:14.000000 slurmgen-3.7.0/LICENSE.txt
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-29 23:48:22.257088 slurmgen-3.7.0/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     2093 2024-03-30 02:44:17.000000 slurmgen-3.7.0/README.md
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-29 23:48:22.253088 slurmgen-3.7.0/example/
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-29 23:48:22.253088 slurmgen-3.7.0/example/data_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-29 00:40:40.000000 slurmgen-3.7.0/example/data_output/goodbye.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       55 2024-05-29 00:40:40.000000 slurmgen-3.7.0/example/data_output/hello.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      756 2024-05-22 21:53:10.000000 slurmgen-3.7.0/example/job_def.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       57 2024-05-22 21:27:31.000000 slurmgen-3.7.0/example/job_tmpl.json
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1063 2024-05-24 14:52:38.000000 slurmgen-3.7.0/example/run_slurm.py
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-29 23:48:22.253088 slurmgen-3.7.0/example/slurm_output/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      692 2024-05-29 00:40:40.000000 slurmgen-3.7.0/example/slurm_output/test.log
+-rwxrw-r--   0 tguillod  (1000) tguillod  (1000)     1252 2024-05-29 00:40:40.000000 slurmgen-3.7.0/example/slurm_output/test.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     1566 2024-05-03 05:50:27.000000 slurmgen-3.7.0/pyproject.toml
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     1719 2023-11-27 16:21:41.000000 slurmgen-3.7.0/run_release.sh
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       38 2024-05-29 23:48:22.257088 slurmgen-3.7.0/setup.cfg
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-29 23:48:22.257088 slurmgen-3.7.0/slurmgen/
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      176 2024-05-24 14:43:56.000000 slurmgen-3.7.0/slurmgen/__init__.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7878 2024-05-29 00:41:06.000000 slurmgen-3.7.0/slurmgen/gen.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)     3277 2024-05-29 23:39:08.000000 slurmgen-3.7.0/slurmgen/run.py
+-rwxrwxr-x   0 tguillod  (1000) tguillod  (1000)     7461 2024-05-24 14:52:38.000000 slurmgen-3.7.0/slurmgen/script.py
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        5 2024-05-29 23:48:22.000000 slurmgen-3.7.0/slurmgen/version.txt
+drwxrwxr-x   0 tguillod  (1000) tguillod  (1000)        0 2024-05-29 23:48:22.257088 slurmgen-3.7.0/slurmgen.egg-info/
+-rw-r--r--   0 tguillod  (1000) tguillod  (1000)     3106 2024-05-29 23:48:22.000000 slurmgen-3.7.0/slurmgen.egg-info/PKG-INFO
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)      503 2024-05-29 23:48:22.000000 slurmgen-3.7.0/slurmgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        1 2024-05-29 23:48:22.000000 slurmgen-3.7.0/slurmgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)       45 2024-05-29 23:48:22.000000 slurmgen-3.7.0/slurmgen.egg-info/entry_points.txt
+-rw-rw-r--   0 tguillod  (1000) tguillod  (1000)        9 2024-05-29 23:48:22.000000 slurmgen-3.7.0/slurmgen.egg-info/top_level.txt
```

### Comparing `slurmgen-3.6.0/LICENSE.txt` & `slurmgen-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/PKG-INFO` & `slurmgen-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.6.0
+Version: 3.7.0
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

### Comparing `slurmgen-3.6.0/README.md` & `slurmgen-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/example/job_def.json` & `slurmgen-3.7.0/example/job_def.json`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/example/run_slurm.py` & `slurmgen-3.7.0/example/run_slurm.py`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/example/slurm_output/test.log` & `slurmgen-3.7.0/example/slurm_output/test.log`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-================================== test - 05/24/24 14:52:38
+================================== test - 05/29/24 00:40:40
 ==================== PARAM
 JOB TAG      : test
-LOG FILE     : slurm_output/test.log
-SCRIPT FILE  : slurm_output/test.sh
+HOSTNAME     : l380
 ==================== TIME
-DATE GEN     : 05/24/24 14:52:38
-DATE RUN     : 05/24/24 14:52:38
+DATE GEN     : 05/28/24 : 20:40:40
+DATE RUN     : 05/28/24 : 20:40:40
 ==================== SLURM
-JOB ID       : NOT SLURM
-JOB NAME     : NOT SLURM
-JOB NODE     : NOT SLURM
-==================== ENV VAR
+JOB ID       : LOCAL
+JOB NAME     : LOCAL
+JOB NODE     : LOCAL
 ==================== RUN: version
 Python 3.10.12
 ==================== RUN: hello
 enter script
 enter script
     ARGUMENT = hello world!
     VARWORLD = Welcome to everyone
 exit script
 ==================== RUN: goodbye
 enter script
 enter script
     ARGUMENT = goodbye world!
     VARWORLD = Welcome to everyone
 exit script
-================================== test - 05/24/24 14:52:38
+================================== test - 05/29/24 00:40:40
```

### Comparing `slurmgen-3.6.0/pyproject.toml` & `slurmgen-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/run_release.sh` & `slurmgen-3.7.0/run_release.sh`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/slurmgen/gen.py` & `slurmgen-3.7.0/slurmgen/gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 __author__ = "Thomas Guillod"
 __copyright__ = "Thomas Guillod - Dartmouth College"
 __license__ = "BSD License"
 
 import os.path
 import shutil
-import datetime
+import time
 
 
 class GenError(Exception):
     """
     Exception during the script generation.
     """
 
@@ -61,15 +61,15 @@
     if "output" in pragmas:
         raise GenError("job log is already set by the script")
     if "error" in pragmas:
         raise GenError("job log is already set by the script")
 
     fid.write('#!/bin/bash\n')
     fid.write('\n')
-    fid.write('# ############### define Slurm commands\n')
+    fid.write('# ############### Slurm commands\n')
     fid.write('#SBATCH --job-name="%s"\n' % tag)
     fid.write('#SBATCH --output="%s"\n' % filename_log)
     for tag, val in pragmas.items():
         if (tag is not None) and (val is not None):
             fid.write('#SBATCH --%s="%s"\n' % (tag, val))
     fid.write('\n')
     fid.write('# ############### init exit code\n')
@@ -91,27 +91,26 @@
     filename_script : string
         Path of the script controlling the simulation.
     filename_log : string
         Path of the log file created by during the Slurm job.
     """
 
     # get current timestamp
-    date = datetime.datetime.utcnow()
+    timestamp = int(time.time())
 
     # write the job name, log file, and script file
     fid.write('echo "==================== PARAM"\n')
-    fid.write('echo "JOB TAG      : %s"\n' % tag)
-    fid.write('echo "LOG FILE     : %s"\n' % filename_log)
-    fid.write('echo "SCRIPT FILE  : %s"\n' % filename_script)
+    fid.write(f'echo "JOB TAG      : {tag}"\n')
+    fid.write('echo "HOSTNAME     : $HOSTNAME"\n')
     fid.write('\n')
 
     # write data about the job submission
     fid.write('echo "==================== TIME"\n')
-    fid.write('echo "DATE GEN     : %s"\n' % date.strftime("%D %H:%M:%S"))
-    fid.write('echo "DATE RUN     : `date -u +"%D %H:%M:%S"`"\n')
+    fid.write(f'echo "DATE GEN     : `date -u +"%D : %H:%M:%S" -d @{timestamp}`"\n')
+    fid.write(f'echo "DATE RUN     : `date -u +"%D : %H:%M:%S" -d @$(date -u +%s)`"\n')
     fid.write('\n')
 
     # write the job id, job name, and the assigned node names
     fid.write('echo "==================== SLURM"\n')
     fid.write('echo "JOB ID       : $SLURM_JOB_ID"\n')
     fid.write('echo "JOB NAME     : $SLURM_JOB_NAME"\n')
     fid.write('echo "JOB NODE     : $SLURM_JOB_NODELIST"\n')
@@ -127,15 +126,15 @@
     fid : file
         File descriptor for the script.
     envs : dict
         Dictionary of environment variable to be set and exported.
     """
 
     if envs:
-        fid.write('echo "==================== ENV VAR"\n')
+        fid.write('# ############### environment variables\n')
         for var, val in envs.items():
             if (var is not None) and (val is not None):
                 fid.write('export %s="%s"\n' % (var, val))
         fid.write('\n')
 
 
 def _write_commands(fid, commands):
@@ -185,23 +184,23 @@
     """
 
     # write the data
     with open(filename_script, "w") as fid:
         # write pragmas
         _write_header(fid, tag, filename_log, pragmas)
 
+        # write environment variables
+        _write_envs(fid, envs)
+
         # write script header
         _write_title(fid, tag)
 
         # write summary of the variables
         _write_summary(fid, tag, filename_script, filename_log)
 
-        # write environment variables
-        _write_envs(fid, envs)
-
         # write the commands to be executed
         _write_commands(fid, commands)
 
         # end script footer
         _write_title(fid, tag)
 
         # end script footer
```

### Comparing `slurmgen-3.6.0/slurmgen/run.py` & `slurmgen-3.7.0/slurmgen/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         )
 
         # wait return
         process.wait()
     except OSError as ex:
         raise RunError("command error: %s" % str(ex))
 
-    # check return code
+    # check return code (failure not allowed)
     if process.returncode != 0:
         raise RunError("invalid return code")
 
 
 def _run_cmd_log(command, filename_log, env):
     """
     Run a Slurm script.
@@ -86,16 +86,16 @@
                 fid.flush()
 
         # wait return
         process.wait()
     except OSError as ex:
         raise RunError("command error: %s" % str(ex))
 
-    # check return code
-    if process.returncode != 0:
+    # check return code (failure allowed)
+    if process.returncode >= 0:
         raise RunError("invalid return code")
 
 
 def run_data(filename_script, filename_log, local, cluster):
     """
     Run a Slurm script.
 
@@ -130,16 +130,16 @@
         # run
         _run_cmd_raw(command, env)
 
     # run locally
     if local:
         # find env
         env = os.environ.copy()
-        env["SLURM_JOB_ID"] = "NOT SLURM"
-        env["SLURM_JOB_NAME"] = "NOT SLURM"
-        env["SLURM_JOB_NODELIST"] = "NOT SLURM"
+        env["SLURM_JOB_ID"] = "LOCAL"
+        env["SLURM_JOB_NAME"] = "LOCAL"
+        env["SLURM_JOB_NODELIST"] = "LOCAL"
 
         # find command
         command = [filename_script]
 
         # run
         _run_cmd_log(command, filename_log, env)
```

### Comparing `slurmgen-3.6.0/slurmgen/script.py` & `slurmgen-3.7.0/slurmgen/script.py`

 * *Files identical despite different names*

### Comparing `slurmgen-3.6.0/slurmgen.egg-info/PKG-INFO` & `slurmgen-3.7.0/slurmgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmgen
-Version: 3.6.0
+Version: 3.7.0
 Summary: SlurmGen - Simple Slurm Manager
 Author-email: Thomas Guillod <guillod@otvam.ch>
 Maintainer-email: Thomas Guillod <guillod@otvam.ch>
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/otvam/slurmgen
 Project-URL: Repository, https://github.com/otvam/slurmgen
 Project-URL: Releases, https://github.com/otvam/slurmgen/releases
```

