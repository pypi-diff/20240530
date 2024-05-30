# Comparing `tmp/frida_start-3.0.0.tar.gz` & `tmp/frida_start-3.0.1.tar.gz`

## Comparing `frida_start-3.0.0.tar` & `frida_start-3.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 frida_start-3.0.0/frida_start/__init__.py
--rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 frida_start-3.0.0/frida_start/command.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 frida_start-3.0.0/.gitignore
--rw-r--r--   0        0        0    35815 2020-02-02 00:00:00.000000 frida_start-3.0.0/LICENSE
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 frida_start-3.0.0/README.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 frida_start-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 frida_start-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 frida_start-3.0.1/frida_start/__init__.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 frida_start-3.0.1/frida_start/command.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 frida_start-3.0.1/.gitignore
+-rw-r--r--   0        0        0    35815 2020-02-02 00:00:00.000000 frida_start-3.0.1/LICENSE
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 frida_start-3.0.1/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 frida_start-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 frida_start-3.0.1/PKG-INFO
```

### Comparing `frida_start-3.0.0/frida_start/command.py` & `frida_start-3.0.1/frida_start/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,16 @@
 #!/usr/bin/env python3
 
-"""This script aims to automate the process of starting frida-server
-on an Android device (for now). The script is a part of AndroidTamer
-project and is based on this issue:
-https://github.com/AndroidTamer/Tools_Repository/issues/234.
-
-This script performs following things:
-1. Try to determine the device architecture
-2. Download the frida-server and extract it
-3. Push it to the device and execute it
-4. Save the PID of the process and write it to 'frida.pid' file.
-
-#Todo:
-* Better exception handling.
-* Implement better/robust architecture detection code
-* Implement for more devices
-* Implement the feature to kill frida-server afterwards
-"""
-
 import argparse
 import logging
-import os
 import subprocess
 import sys
 import lzma
 import pathlib
+import time
 
 import requests
 
 from frida_start import __version__
 
 logging.basicConfig(
     stream=sys.stdout,
@@ -39,27 +21,30 @@
 
 try:
     from frida import __version__ as FRIDA_VERSION
 except ImportError:
     log.error("Frida not found. Please run `pip install frida` to proceed.")
     sys.exit(1)
 
-# Just put "adb" below, if adb exists in your system path.
 ADB_PATH = "adb"
 DOWNLOAD_PATH = pathlib.Path.home() / ".frida-start"
+CHUNK_SIZE = 1024 * 10
+GETPROP_ARCHS = {
+    "armeabi": "arm",
+    "armeabi-v7a": "arm",
+    "arm64-v8a": "arm64",
+    "x86": "x86",
+    "x86_64": "x86_64",
+}
 
 
-def list_devices():
-    """
-    Return devices conected to adb
-    :return: list
-    """
+def get_connected_devices() -> dict[str, dict[str, str]]:
     cmd = f"{ADB_PATH} devices -l"
     output = (
-        subprocess.check_output(cmd, shell=True)
+        subprocess.check_output(cmd)
         .strip()
         .decode("utf-8")
         .replace("\r", "")
         .split("\n")
     )
 
     devices = set()
@@ -67,101 +52,63 @@
         device = device.strip()
         if device != "":
             devices.add(tuple(device.split()))
 
     return {d[0]: {t.split(":")[0]: t.split(":")[1] for t in d[2:]} for d in devices}
 
 
-def get_device_arch(transport_id=None):
-    """This function tries to determine the architecture of the device, so that
-    the correct version of Frida-server can be downloaded.
-
-    :returns either "arch" that Frida release page understands or None.
-    """
-    arch = None
-
+def get_device_arch(transport_id: str) -> str:
     getprop_cmd = f"{ADB_PATH} -t {transport_id} shell getprop ro.product.cpu.abi"
-    getprop_archs = ["armeabi", "armeabi-v7a", "arm64-v8a", "x86", "x86_64"]
-    # We know shell=True is bad, but should be fine here.
-    output = (
-        subprocess.check_output(getprop_cmd, shell=True).lower().strip().decode("utf-8")
-    )
-
-    if output in getprop_archs:
-        if output in ["armeabi", "armeabi-v7a"]:
-            arch = "arm"
-        elif output == "arm64-v8a":
-            arch = "arm64"
-        else:
-            arch = output
-
-    return arch
+    output = subprocess.check_output(getprop_cmd).lower().strip().decode("utf-8")
+    if output not in GETPROP_ARCHS:
+        raise RuntimeError("Could not determine device's arch")
+    return GETPROP_ARCHS[output]
 
 
-def prepare_download_url(arch):
-    """Depending upon the arch provided, the function returns the download URL."""
+def get_download_url(arch: str) -> str:
     return f"https://github.com/frida/frida/releases/download/{FRIDA_VERSION}/frida-server-{FRIDA_VERSION}-android-{arch}.xz"
 
 
-def download_and_extract(url, fpath, force_download=False):
-    """This function downloads the given URL, extracts .xz archive
-    as given file name.
-
-    :returns True if successful, else False.
-    """
-    data = None
-    DOWNLOAD_PATH.mkdir(exist_ok=True)
-
-    fpath = DOWNLOAD_PATH / fpath
-
+def download_and_extract(
+    url: str, fpath: pathlib.Path, force_download: bool = False
+) -> None:
     if fpath.is_file() and not force_download:
         log.info(f"Using {fpath.name} from downloaded cache")
-        return True
+        return
 
-    log.warning(f"Downloading: {url}")
+    fpath.parent.mkdir(exist_ok=True)
+    data = None
+
+    log.info(f"Downloading: {url}")
     req = requests.get(url, stream=True)
-    if req.status_code == 200:
-        # Downloading and writing the archive.
-        archive_name = fpath.with_suffix(".xz")
-
-        req.raw.decode_content = True
-        with open(archive_name, "wb") as fh:
-            for chunk in req.iter_content(1024):
-                fh.write(chunk)
+    req.raise_for_status()
 
-        with lzma.open(archive_name) as fh:
-            data = fh.read()
+    archive_path = fpath.with_suffix(".xz")
 
-        os.unlink(archive_name)
-    else:
-        log.error(
-            f"ERROR: downloading frida-server. Got HTTP status code {req.status_code} from server."
-        )
+    req.raw.decode_content = True
+    with open(archive_path, "wb") as fh:
+        for chunk in req.iter_content(CHUNK_SIZE):
+            fh.write(chunk)
 
-    if data:
-        log.info(f"Writing file as: {fpath}")
-        fpath.write_bytes(data)
-        return True
-    return False
+    with lzma.open(archive_path) as fh:
+        data = fh.read()
 
+    archive_path.unlink()
 
-def push_and_execute(fname, transport_id=None):
-    """This function pushes the file to device, makes it executable,
-    and then finally runs the binary. The function also saves the PID
-    of process in 'frida.pid' file.
-    """
+    log.info(f"Writing file to {fpath}")
+    fpath.write_bytes(data)
 
-    fname = DOWNLOAD_PATH / fname
 
+def push_and_execute(fpath: pathlib.Path, transport_id: str) -> None:
     push_cmd = [
         ADB_PATH,
         "-t",
         transport_id,
         "push",
-        str(fname),
+        str(fpath),
         "/data/local/tmp/frida-server",
     ]
     chmod_cmd = [
         ADB_PATH,
         "-t",
         transport_id,
         "shell",
@@ -178,14 +125,15 @@
         "frida-server",
     ]
     execute_cmd = [
         ADB_PATH,
         "-t",
         transport_id,
         "shell",
+        "nohup",
         "su",
         "0",
         "/data/local/tmp/frida-server",
     ]
 
     res = subprocess.Popen(push_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     res.wait()
@@ -200,60 +148,63 @@
     subprocess.Popen(chmod_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE).wait()
 
     log.info("Killing all frida-server on device.")
     subprocess.Popen(kill_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE).wait()
 
     log.info("Executing frida-server on device.")
     res = subprocess.Popen(execute_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    ret_code = None
-    try:
-        ret_code = res.wait(3)
-    except:
-        pass
-
+    time.sleep(3)
+    ret_code = res.poll()
     if ret_code is not None and ret_code != 0:
         decoded = res.stderr.readline().decode("utf-8")
-        log.error(f"Error executing frida-server. {decoded}")
+        msg = f"Error executing frida-server. {decoded}"
+        log.error(msg)
+        raise RuntimeError(msg)
+    res.kill()
 
 
-def main():
-    """This function is where the magic happens."""
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument("-d", "--device-name", required=False)
     parser.add_argument(
         "-f", "--force", help="force download", action="store_true", default=False
     )
-    parser.add_argument("--version", action="version", version=__version__)
-    ops = parser.parse_args()
+    parser.add_argument("-V", "--version", action="version", version=__version__)
+    return parser.parse_args()
+
 
-    devices = list_devices()
+def main():
+    args = parse_args()
+
+    devices = get_connected_devices()
     if len(devices) == 0:
         log.error("No device found. Exiting.")
-        sys.exit(1)
+        return 1
 
-    log.info("Devices: {}".format(", ".join([dname for dname, _ in devices.items()])))
+    log.info("Devices: {}".format(", ".join(devices.keys())))
 
-    if len(devices) != 1 and ops.device_name is None:
-        parser.exit(2, "Multiple devices conected select one with -d\n")
-    elif ops.device_name is not None and ops.device_name not in devices:
-        parser.exit(2, f"Device {ops.device_name} not found\n")
+    if len(devices) != 1 and args.device_name is None:
+        log.error("Multiple devices conected select one with -d")
+        return 1
+    elif args.device_name is not None and args.device_name not in devices:
+        log.error(f"Device {args.device_name} not found")
+        return 1
 
-    if ops.device_name is None:
-        ops.device_name, _ = next(iter(devices.items()), None)
+    if args.device_name is None:
+        args.device_name = next(iter(devices.keys()), None)
 
     log.info(f"Current installed Frida version: {FRIDA_VERSION}")
 
-    transport_id = devices[ops.device_name]["transport_id"]
+    transport_id = devices[args.device_name]["transport_id"]
     arch = get_device_arch(transport_id=transport_id)
+    log.info(f"Found arch: {arch}")
+
+    url = get_download_url(arch)
+    fpath = DOWNLOAD_PATH / f"frida-server-{FRIDA_VERSION}-android-{arch}"
 
-    if arch:
-        log.info(f"Found arch: {arch}")
-        url = prepare_download_url(arch)
-        fname = f"frida-server-{FRIDA_VERSION}-android-{arch}"
-        if download_and_extract(url, fname, ops.force):
-            push_and_execute(fname, transport_id=transport_id)
-    else:
-        log.info("Could not determine device's arch. Exiting.")
+    download_and_extract(url, fpath, args.force)
+    push_and_execute(fpath, transport_id=transport_id)
+    return 0
 
 
 if __name__ == "__main__":
-    main()
+    sys.exit(main())
```

### Comparing `frida_start-3.0.0/.gitignore` & `frida_start-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `frida_start-3.0.0/LICENSE` & `frida_start-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frida_start-3.0.0/pyproject.toml` & `frida_start-3.0.1/pyproject.toml`

 * *Files identical despite different names*

