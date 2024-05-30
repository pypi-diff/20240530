# Comparing `tmp/i3_find_or_open-0.6.1.tar.gz` & `tmp/i3_find_or_open-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3_find_or_open-0.6.1.tar", max compression
+gzip compressed data, was "i3_find_or_open-0.6.2.tar", max compression
```

## Comparing `i3_find_or_open-0.6.1.tar` & `i3_find_or_open-0.6.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-11-01 21:50:10.472238 i3_find_or_open-0.6.1/LICENSE
--rw-r--r--   0        0        0     2415 2023-11-23 22:50:53.458219 i3_find_or_open-0.6.1/README.md
--rwxr-xr-x   0        0        0     3139 2024-05-30 13:53:54.927616 i3_find_or_open-0.6.1/i3_find_or_open/main.py
--rw-r--r--   0        0        0      543 2024-05-30 13:53:54.927616 i3_find_or_open-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 i3_find_or_open-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-01 21:50:10.472238 i3_find_or_open-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2757 2024-05-30 14:02:38.081899 i3_find_or_open-0.6.2/README.md
+-rwxr-xr-x   0        0        0     3139 2024-05-30 13:53:54.927616 i3_find_or_open-0.6.2/i3_find_or_open/main.py
+-rw-r--r--   0        0        0      543 2024-05-30 14:03:01.178579 i3_find_or_open-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 i3_find_or_open-0.6.2/PKG-INFO
```

### Comparing `i3_find_or_open-0.6.1/LICENSE` & `i3_find_or_open-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `i3_find_or_open-0.6.1/README.md` & `i3_find_or_open-0.6.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,72 @@
 # i3-find-or-open
-This repo provides a command-line tool: `i3-find-or-open` that can find a window by regex in your i3wm instance, and display it, or execute any command if it is not open.
 
-It is intended to help you bind keys that will reliably show you a window, whether or not it is open already, but technically it is capable of showing you any window (which is uniquely identifiable by either title or class), or running an arbitrary command if it is not open.
+This repo provides a command-line tool: `i3-find-or-open` that can find a
+window by regex in your i3wm instance, and display it, or execute any command
+if it is not open.
+
+It is intended to help you bind keys that will reliably show you a window,
+whether or not it is open already, but technically it is capable of showing you
+any window (which is uniquely identifiable by either title or class), or
+running an arbitrary command if it is not open.
+
 ## Installation
-i3-find-or-open is available on [PyPI](https://pypi.org/project/i3_find_or_open/), and the best way to install it (if you don't want to break your system python installation) is to use [pipx](https://pypa.github.io/pipx/installation/) (N.B. there is an Arch package `python-pipx` to install this with). 
-```
+
+i3-find-or-open is available on
+[PyPI](https://pypi.org/project/i3_find_or_open/), and the best way to install
+it (if you don't want to break your system python installation) is to use
+[pipx](https://pypa.github.io/pipx/installation/) (N.B. there is an Arch
+package `python-pipx` to install this with).
+
+```sh
 pipx install i3-find-or-open
 ```
-Note that if you want to bind keys in i3 to this program, it will need to be installed for all users:
-```
+
+Note that if you want to bind keys in i3 to this program, it will need to be
+installed for all users:
+
+```sh
 sudo PIPX_HOME=/opt/pipx PIPX_BIN_DIR=/usr/local/bin pipx install i3-find-or-open
 ```
-*(or you could bind `$HOME/.local/bin/i3-find-or-open` if you'd rather not install it for everybody)*
 
-If you do want to risk breaking your system python, you could just use `pip`. 
+*(or you could bind `$HOME/.local/bin/i3-find-or-open` if you'd rather not
+install it for everybody)*
+
+If you do want to risk breaking your system python, you could just use `pip`.
 
-Or, you could install it in a virtual environment yourself (note that this is all `pipx` is doing, but you might rather manage these environments manually).
+Or, you could install it in a virtual environment yourself (note that this is
+all `pipx` is doing, but you might rather manage these environments manually).
 
 ## Usage
-Let's say I wanted to use this to bind `$mod+o` to open my Obsidian vault (called "vault"):
-```
+
+Let's say I wanted to use this to bind `$mod+o` to open my Obsidian vault
+(called "vault"):
+
+```i3config
 bindsym $mod+o exec --no-startup-id "i3-find-or-open '^.* - vault - Obsidian v([1-9]|\.)+$' 'obsidian'"
 ```
-It's worth noting that the title regex you use will usually have to be quite specific when running from a command line, as the title of your terminal emulator will likely include the full command string (make use of `^`, and `$` tokens where possible).
+
+It's worth noting that the title regex you use will usually have to be quite
+specific when running from a command line, as the title of your terminal
+emulator will likely include the full command string (make use of `^`, and `$`
+tokens where possible).
 
 Some other examples, taken from my i3 config:
-```
+
+```i3config
 bindsym $mod+t exec --no-startup-id "i3-find-or-open 'timetable\.ods — LibreOffice Calc' 'libreoffice --norestore ~/icl/timetable.ods'"
 bindsym $mod+q exec --no-startup-id "i3-find-or-open 'qBittorrent' 'qbittorrent'"
 ```
 
-You can also use the `-c` flag to match a window class instead of title if the title completely changes (like for the Spotify app).
+You can also use the `-c` flag to match a window class instead of title if the
+title completely changes (like for the Spotify app).
 
-```
+```i3config
 bindsym $mod+s exec --no-startup-id "i3-find-or-open -c 'Spotify' 'spotify-launcher'"
 ```
 
+You can use the `-t` flag to toggle scratchpad windows (i.e. to mimic the
+effect of the `scratchpad show` command, but just for your targeted window).
+Keeping this off (as is the default) will make sure the behaviour is such that
+your keybinding will always show you the targeted window, no matter what.
+
 Title and class information about any open window can be found with the `xprop` command.
```

### Comparing `i3_find_or_open-0.6.1/i3_find_or_open/main.py` & `i3_find_or_open-0.6.2/i3_find_or_open/main.py`

 * *Files identical despite different names*

### Comparing `i3_find_or_open-0.6.1/pyproject.toml` & `i3_find_or_open-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "i3_find_or_open"
-version = "0.6.1"
+version = "0.6.2"
 license = "GPL-3.0-only"
 description = "A command-line utility that helps you bind keys to find and display a window, or open it if there is no instance running in i3wm."
 authors = ["Hector Brown <hectorjbrown@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `i3_find_or_open-0.6.1/PKG-INFO` & `i3_find_or_open-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,89 @@
 Metadata-Version: 2.1
 Name: i3_find_or_open
-Version: 0.6.1
+Version: 0.6.2
 Summary: A command-line utility that helps you bind keys to find and display a window, or open it if there is no instance running in i3wm.
 License: GPL-3.0-only
 Author: Hector Brown
 Author-email: hectorjbrown@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: i3ipc (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # i3-find-or-open
-This repo provides a command-line tool: `i3-find-or-open` that can find a window by regex in your i3wm instance, and display it, or execute any command if it is not open.
 
-It is intended to help you bind keys that will reliably show you a window, whether or not it is open already, but technically it is capable of showing you any window (which is uniquely identifiable by either title or class), or running an arbitrary command if it is not open.
+This repo provides a command-line tool: `i3-find-or-open` that can find a
+window by regex in your i3wm instance, and display it, or execute any command
+if it is not open.
+
+It is intended to help you bind keys that will reliably show you a window,
+whether or not it is open already, but technically it is capable of showing you
+any window (which is uniquely identifiable by either title or class), or
+running an arbitrary command if it is not open.
+
 ## Installation
-i3-find-or-open is available on [PyPI](https://pypi.org/project/i3_find_or_open/), and the best way to install it (if you don't want to break your system python installation) is to use [pipx](https://pypa.github.io/pipx/installation/) (N.B. there is an Arch package `python-pipx` to install this with). 
-```
+
+i3-find-or-open is available on
+[PyPI](https://pypi.org/project/i3_find_or_open/), and the best way to install
+it (if you don't want to break your system python installation) is to use
+[pipx](https://pypa.github.io/pipx/installation/) (N.B. there is an Arch
+package `python-pipx` to install this with).
+
+```sh
 pipx install i3-find-or-open
 ```
-Note that if you want to bind keys in i3 to this program, it will need to be installed for all users:
-```
+
+Note that if you want to bind keys in i3 to this program, it will need to be
+installed for all users:
+
+```sh
 sudo PIPX_HOME=/opt/pipx PIPX_BIN_DIR=/usr/local/bin pipx install i3-find-or-open
 ```
-*(or you could bind `$HOME/.local/bin/i3-find-or-open` if you'd rather not install it for everybody)*
 
-If you do want to risk breaking your system python, you could just use `pip`. 
+*(or you could bind `$HOME/.local/bin/i3-find-or-open` if you'd rather not
+install it for everybody)*
+
+If you do want to risk breaking your system python, you could just use `pip`.
 
-Or, you could install it in a virtual environment yourself (note that this is all `pipx` is doing, but you might rather manage these environments manually).
+Or, you could install it in a virtual environment yourself (note that this is
+all `pipx` is doing, but you might rather manage these environments manually).
 
 ## Usage
-Let's say I wanted to use this to bind `$mod+o` to open my Obsidian vault (called "vault"):
-```
+
+Let's say I wanted to use this to bind `$mod+o` to open my Obsidian vault
+(called "vault"):
+
+```i3config
 bindsym $mod+o exec --no-startup-id "i3-find-or-open '^.* - vault - Obsidian v([1-9]|\.)+$' 'obsidian'"
 ```
-It's worth noting that the title regex you use will usually have to be quite specific when running from a command line, as the title of your terminal emulator will likely include the full command string (make use of `^`, and `$` tokens where possible).
+
+It's worth noting that the title regex you use will usually have to be quite
+specific when running from a command line, as the title of your terminal
+emulator will likely include the full command string (make use of `^`, and `$`
+tokens where possible).
 
 Some other examples, taken from my i3 config:
-```
+
+```i3config
 bindsym $mod+t exec --no-startup-id "i3-find-or-open 'timetable\.ods — LibreOffice Calc' 'libreoffice --norestore ~/icl/timetable.ods'"
 bindsym $mod+q exec --no-startup-id "i3-find-or-open 'qBittorrent' 'qbittorrent'"
 ```
 
-You can also use the `-c` flag to match a window class instead of title if the title completely changes (like for the Spotify app).
+You can also use the `-c` flag to match a window class instead of title if the
+title completely changes (like for the Spotify app).
 
-```
+```i3config
 bindsym $mod+s exec --no-startup-id "i3-find-or-open -c 'Spotify' 'spotify-launcher'"
 ```
 
+You can use the `-t` flag to toggle scratchpad windows (i.e. to mimic the
+effect of the `scratchpad show` command, but just for your targeted window).
+Keeping this off (as is the default) will make sure the behaviour is such that
+your keybinding will always show you the targeted window, no matter what.
+
 Title and class information about any open window can be found with the `xprop` command.
```

