# Comparing `tmp/colomoto_docker-8.3.tar.gz` & `tmp/colomoto_docker-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colomoto_docker-8.3.tar", last modified: Wed May 29 06:38:44 2024, max compression
+gzip compressed data, was "colomoto_docker-9.0.tar", last modified: Wed May 29 20:04:24 2024, max compression
```

## Comparing `colomoto_docker-8.3.tar` & `colomoto_docker-9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2024-05-29 06:38:44.913926 colomoto_docker-8.3/
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)      245 2024-05-29 06:38:44.913926 colomoto_docker-8.3/PKG-INFO
-drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2024-05-29 06:38:44.912926 colomoto_docker-8.3/colomoto_docker.egg-info/
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)       27 2024-05-29 06:38:44.000000 colomoto_docker-8.3/colomoto_docker.egg-info/SOURCES.txt
--rwxr-xr-x   0 pauleve   (1000) pauleve   (1000)    11376 2024-05-29 06:37:35.000000 colomoto_docker-8.3/colomoto_docker.py
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)       38 2024-05-29 06:38:44.913926 colomoto_docker-8.3/setup.cfg
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)      645 2023-10-19 22:28:21.000000 colomoto_docker-8.3/setup.py
+drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2024-05-29 20:04:24.614133 colomoto_docker-9.0/
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)      245 2024-05-29 20:04:24.614133 colomoto_docker-9.0/PKG-INFO
+drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2024-05-29 20:04:24.613133 colomoto_docker-9.0/colomoto_docker.egg-info/
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)       27 2024-05-29 20:04:24.000000 colomoto_docker-9.0/colomoto_docker.egg-info/SOURCES.txt
+-rwxr-xr-x   0 pauleve   (1000) pauleve   (1000)    11926 2024-05-29 20:04:10.000000 colomoto_docker-9.0/colomoto_docker.py
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)       38 2024-05-29 20:04:24.615133 colomoto_docker-9.0/setup.cfg
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)      645 2023-10-19 22:28:21.000000 colomoto_docker-9.0/setup.py
```

### Comparing `colomoto_docker-8.3/colomoto_docker.py` & `colomoto_docker-9.0/colomoto_docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import random
 import re
 import socket
 import subprocess
 import sys
 import webbrowser
 
-__version__ = "8.3"
+__version__ = "9.0"
 
 on_linux = platform.system() == "Linux"
 
 pat_tag = re.compile(r"\d{4}-\d{2}-\d{2}")
 
 persistent_volume = "colomoto-{}".format(getuser())
 persistent_dir = "persistent"
@@ -83,16 +83,14 @@
     parser = ArgumentParser()
     parser.add_argument("--bind", default=None, type=str,
         help="Bind specified path to the docker working directory")
     parser.add_argument("--no-selinux", default=False, action="store_true",
         help="Disable SElinux for this container")
     parser.add_argument("-w", "--workdir", default="/notebook", type=str,
         help="Workdir within the docker image")
-    parser.add_argument("--shell", default=False, action="store_true",
-        help="Start interactive shell instead of notebook service")
     parser.add_argument("-V", "--version", type=str, default="same",
         help="""Version of docker image ('latest' to fetch the latest tag;
         'same' for most recently fetched image)""")
     parser.add_argument("--port", default=0, type=int,
         help="Local port")
     parser.add_argument("--image", default=official_image,
         help="Docker image")
@@ -101,27 +99,34 @@
     parser.add_argument("--unsafe-ssl", default=False, action="store_true",
         help="Do not check for SSL certificates")
     parser.add_argument("--no-update", default=False, action="store_true",
         help="Do not check for image update")
     parser.add_argument("--cleanup", default=False, action="store_true",
         help="Cleanup old images")
 
+    group = parser.add_argument_group("choice of interface")
+    x = group.add_mutually_exclusive_group()
+    x.add_argument('--lab', action='store_true', help="Use jupyter lab interface")
+    x.add_argument('--notebook', action='store_false', help="Use jupyter notebook interface")
+    x.add_argument("--shell", default=False, action="store_true",
+        help="Start interactive shell instead of notebook service")
+
     group = parser.add_argument_group("docker run options")
     group.add_argument("-e", "--env", action="append",
         help="Set environment variables")
     group.add_argument("--name", help="Name of the container")
     group.add_argument("-v", "--volume", action="append",
         help="Bind mount a volume")
     group.add_argument("--network", type=str,
         help="Network access")
     group.add_argument("--ulimit", type=str,
         help="Resource limit")
     docker_run_opts = ["env", "volume", "network", "ulimit"]
 
-    parser.add_argument("command", nargs=REMAINDER, help="Command to run instead of colomoto-nb")
+    parser.add_argument("command", nargs=REMAINDER, help="Command to run in place of web interface")
     args = parser.parse_args()
 
     info(f"colomoto-docker {__version__}")
 
     image_tag = args.version
 
     if args.version == "same":
@@ -261,16 +266,24 @@
                     if opt == "volume":
                         v = easy_volume(v)
                     argv += ["--%s"%opt, v]
             else:
                 argv += ["--%s" % opt, val]
 
     argv += [image]
+
+    _args_jupyter = ["--no-browser", "--port", "8888",
+                        "--ip", "0.0.0.0", "--NotebookApp.token="]
+
     if args.shell:
         argv += ["bash"]
+    elif args.lab:
+        argv += ["jupyter-lab"] + _args_jupyter
+    elif args.notebook:
+        argv += ["jupyter-notebook"] + _args_jupyter
     elif args.command:
         argv += args.command
 
     info("# %s" % " ".join(argv))
 
     if not args.shell and not args.command and not args.no_browser:
         if os.fork() == 0:
```

### Comparing `colomoto_docker-8.3/setup.py` & `colomoto_docker-9.0/setup.py`

 * *Files identical despite different names*

