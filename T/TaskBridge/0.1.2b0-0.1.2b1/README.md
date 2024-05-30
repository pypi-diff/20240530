# Comparing `tmp/taskbridge-0.1.2b0.tar.gz` & `tmp/taskbridge-0.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbridge-0.1.2b0.tar", max compression
+gzip compressed data, was "taskbridge-0.1.2b1.tar", max compression
```

## Comparing `taskbridge-0.1.2b0.tar` & `taskbridge-0.1.2b1.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    35128 2024-05-29 14:46:38.637192 taskbridge-0.1.2b0/LICENSE
--rw-r--r--   0        0        0     7735 2024-05-29 14:46:38.637482 taskbridge-0.1.2b0/README.md
--rw-r--r--   0        0        0     1703 2024-05-29 14:46:38.665234 taskbridge-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0      348 2024-05-29 14:46:38.665748 taskbridge-0.1.2b0/taskbridge/__init__.py
--rw-r--r--   0        0        0      138 2024-05-29 14:46:38.665940 taskbridge-0.1.2b0/taskbridge/cli/__init__.py
--rw-r--r--   0        0        0    19064 2024-05-29 14:46:38.666121 taskbridge-0.1.2b0/taskbridge/cli/tbcli.py
--rw-r--r--   0        0        0      915 2024-05-29 14:46:38.666360 taskbridge-0.1.2b0/taskbridge/gui/TaskBridge.py
--rw-r--r--   0        0        0      429 2024-05-29 14:46:38.666525 taskbridge-0.1.2b0/taskbridge/gui/__init__.py
--rw-r--r--   0        0        0     2844 2024-05-29 14:46:38.666722 taskbridge-0.1.2b0/taskbridge/gui/about.ui
--rw-r--r--   0        0        0    13473 2024-05-29 14:46:38.667068 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png
--rw-r--r--   0        0        0    13805 2024-05-29 14:46:38.667348 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png
--rw-r--r--   0        0        0   772414 2024-05-29 14:46:38.668877 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png
--rw-r--r--   0        0        0    16622 2024-05-29 14:46:38.671068 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png
--rw-r--r--   0        0        0    17860 2024-05-29 14:46:38.671293 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png
--rw-r--r--   0        0        0    19866 2024-05-29 14:46:38.672912 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png
--rw-r--r--   0        0        0    23814 2024-05-29 14:46:38.673433 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png
--rw-r--r--   0        0        0    25818 2024-05-29 14:46:38.673746 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png
--rw-r--r--   0        0        0      822 2024-05-29 14:46:38.674051 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png
--rw-r--r--   0        0        0    30211 2024-05-29 14:46:38.674423 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png
--rw-r--r--   0        0        0    31652 2024-05-29 14:46:38.674781 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png
--rw-r--r--   0        0        0    34032 2024-05-29 14:46:38.675263 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png
--rw-r--r--   0        0        0    39070 2024-05-29 14:46:38.675737 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png
--rw-r--r--   0        0        0     1104 2024-05-29 14:46:38.675995 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png
--rw-r--r--   0        0        0    45736 2024-05-29 14:46:38.676540 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png
--rw-r--r--   0        0        0    60912 2024-05-29 14:46:38.676837 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png
--rw-r--r--   0        0        0     1922 2024-05-29 14:46:38.677079 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png
--rw-r--r--   0        0        0     2235 2024-05-29 14:46:38.677318 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png
--rw-r--r--   0        0        0     3180 2024-05-29 14:46:38.677584 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png
--rw-r--r--   0        0        0     4265 2024-05-29 14:46:38.677806 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png
--rw-r--r--   0        0        0     4543 2024-05-29 14:46:38.678020 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png
--rw-r--r--   0        0        0   206946 2024-05-29 14:46:38.678816 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png
--rw-r--r--   0        0        0     5252 2024-05-29 14:46:38.679026 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png
--rw-r--r--   0        0        0     5549 2024-05-29 14:46:38.679300 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png
--rw-r--r--   0        0        0     5649 2024-05-29 14:46:38.679428 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png
--rw-r--r--   0        0        0     5983 2024-05-29 14:46:38.679630 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png
--rw-r--r--   0        0        0     6583 2024-05-29 14:46:38.679855 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png
--rw-r--r--   0        0        0     6988 2024-05-29 14:46:38.679989 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png
--rw-r--r--   0        0        0     7993 2024-05-29 14:46:38.680118 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png
--rw-r--r--   0        0        0     8732 2024-05-29 14:46:38.680349 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png
--rw-r--r--   0        0        0     9417 2024-05-29 14:46:38.680628 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png
--rw-r--r--   0        0        0    10705 2024-05-29 14:46:38.680861 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png
--rw-r--r--   0        0        0    10894 2024-05-29 14:46:38.680985 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png
--rw-r--r--   0        0        0    11674 2024-05-29 14:46:38.681115 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png
--rw-r--r--   0        0        0     7139 2024-05-29 14:46:38.681329 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0   772414 2024-05-29 14:46:38.681942 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/appstore.png
--rw-r--r--   0        0        0   214701 2024-05-29 14:46:38.682811 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/playstore.png
--rw-r--r--   0        0        0   998221 2024-05-29 14:46:38.685300 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.icns
--rw-r--r--   0        0        0    17569 2024-05-29 14:46:38.685768 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png
--rw-r--r--   0        0        0    50656 2024-05-29 14:46:38.686088 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png
--rw-r--r--   0        0        0     1699 2024-05-29 14:46:38.686298 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png
--rw-r--r--   0        0        0     2759 2024-05-29 14:46:38.686540 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png
--rw-r--r--   0        0        0    50655 2024-05-29 14:46:38.686841 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png
--rw-r--r--   0        0        0   159642 2024-05-29 14:46:38.687387 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png
--rw-r--r--   0        0        0     2759 2024-05-29 14:46:38.687491 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png
--rw-r--r--   0        0        0     6510 2024-05-29 14:46:38.689300 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png
--rw-r--r--   0        0        0   159641 2024-05-29 14:46:38.691223 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png
--rw-r--r--   0        0        0   551167 2024-05-29 14:46:38.692610 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png
--rw-r--r--   0        0        0   931253 2024-05-29 14:46:38.696537 taskbridge-0.1.2b0/taskbridge/gui/assets/source/TaskBridge_Icon.xcf
--rw-r--r--   0        0        0    69368 2024-05-29 14:46:38.697232 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge.xcf
--rw-r--r--   0        0        0   658861 2024-05-29 14:46:38.698526 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_black.xcf
--rw-r--r--   0        0        0    63732 2024-05-29 14:46:38.698922 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_optimised.xcf
--rw-r--r--   0        0        0  1156034 2024-05-29 14:46:38.700882 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_white.xcf
--rw-r--r--   0        0        0   710088 2024-05-29 14:46:38.705680 taskbridge-0.1.2b0/taskbridge/gui/assets/source/dmg_background.png
--rw-r--r--   0        0        0     3862 2024-05-29 14:46:38.705979 taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png
--rw-r--r--   0        0        0     5539 2024-05-29 14:46:38.706230 taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-swap-7-512.png
--rw-r--r--   0        0        0     8361 2024-05-29 14:46:38.706503 taskbridge-0.1.2b0/taskbridge/gui/assets/source/local.png
--rw-r--r--   0        0        0     2197 2024-05-29 14:46:38.706759 taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_black.xcf
--rw-r--r--   0        0        0     3294 2024-05-29 14:46:38.707000 taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_white.xcf
--rw-r--r--   0        0        0    18816 2024-05-29 14:46:38.707358 taskbridge-0.1.2b0/taskbridge/gui/assets/source/remote.png
--rw-r--r--   0        0        0   825227 2024-05-29 14:46:38.709311 taskbridge-0.1.2b0/taskbridge/gui/assets/source/tb_disk_icon.icns
--rw-r--r--   0        0        0     1301 2024-05-29 14:46:38.709605 taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_black.png
--rw-r--r--   0        0        0     1301 2024-05-29 14:46:38.709828 taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_white.png
--rw-r--r--   0        0        0     1591 2024-05-29 14:46:38.710039 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_black.png
--rw-r--r--   0        0        0     1686 2024-05-29 14:46:38.710255 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_white.png
--rw-r--r--   0        0        0      965 2024-05-29 14:46:38.710478 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_black.png
--rw-r--r--   0        0        0     1950 2024-05-29 14:46:38.710713 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_black.png
--rw-r--r--   0        0        0     1955 2024-05-29 14:46:38.710919 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_white.png
--rw-r--r--   0        0        0      990 2024-05-29 14:46:38.711119 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_white.png
--rw-r--r--   0        0        0     1266 2024-05-29 14:46:38.711316 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_black.png
--rw-r--r--   0        0        0     2885 2024-05-29 14:46:38.711498 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_black.png
--rw-r--r--   0        0        0     2847 2024-05-29 14:46:38.711688 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_white.png
--rw-r--r--   0        0        0     1290 2024-05-29 14:46:38.711895 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_white.png
--rw-r--r--   0        0        0    17458 2024-05-29 14:46:38.712296 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_black.gif
--rw-r--r--   0        0        0    17522 2024-05-29 14:46:38.712703 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_white.gif
--rw-r--r--   0        0        0    47984 2024-05-29 14:46:38.713321 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_black.png
--rw-r--r--   0        0        0    11350 2024-05-29 14:46:38.713556 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_white.png
--rw-r--r--   0        0        0   387868 2024-05-29 14:46:38.714712 taskbridge-0.1.2b0/taskbridge/gui/assets/ui/TaskBridge.png
--rw-r--r--   0        0        0     4909 2024-05-29 14:46:38.714953 taskbridge-0.1.2b0/taskbridge/gui/assets/ui/refresh.png
--rw-r--r--   0        0        0     3701 2024-05-29 14:46:38.715142 taskbridge-0.1.2b0/taskbridge/gui/assets/ui/trash.png
--rw-r--r--   0        0        0    29098 2024-05-29 14:46:38.715349 taskbridge-0.1.2b0/taskbridge/gui/taskbridge.ui
--rw-r--r--   0        0        0      908 2024-05-29 14:46:38.715578 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/__init__.py
--rw-r--r--   0        0        0      476 2024-05-29 14:46:38.715766 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/mainwindow.py
--rw-r--r--   0        0        0     2703 2024-05-29 14:46:38.715983 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/notecheckbox.py
--rw-r--r--   0        0        0     1918 2024-05-29 14:46:38.716193 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/remindercheckbox.py
--rw-r--r--   0        0        0    46116 2024-05-29 14:46:38.716516 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/taskbridgeapp.py
--rw-r--r--   0        0        0    13063 2024-05-29 14:46:38.716812 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/threadedtasks.py
--rw-r--r--   0        0        0     1771 2024-05-29 14:46:38.717003 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/trayicon.py
--rw-r--r--   0        0        0     3201 2024-05-29 14:46:38.717196 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_aboutwindow.py
--rw-r--r--   0        0        0    32872 2024-05-29 14:46:38.717415 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_mainwindow.py
--rw-r--r--   0        0        0     5496 2024-05-29 14:46:38.717636 taskbridge-0.1.2b0/taskbridge/helpers.py
--rw-r--r--   0        0        0      570 2024-05-29 14:46:38.717839 taskbridge-0.1.2b0/taskbridge/notes/__init__.py
--rw-r--r--   0        0        0     7391 2024-05-29 14:46:38.718013 taskbridge-0.1.2b0/taskbridge/notes/controller.py
--rw-r--r--   0        0        0      572 2024-05-29 14:46:38.718265 taskbridge-0.1.2b0/taskbridge/notes/model/__init__.py
--rw-r--r--   0        0        0    19383 2024-05-29 14:46:38.718466 taskbridge-0.1.2b0/taskbridge/notes/model/note.py
--rw-r--r--   0        0        0    43723 2024-05-29 14:46:38.718734 taskbridge-0.1.2b0/taskbridge/notes/model/notefolder.py
--rw-r--r--   0        0        0     6063 2024-05-29 14:46:38.718887 taskbridge-0.1.2b0/taskbridge/notes/model/notescript.py
--rw-r--r--   0        0        0      651 2024-05-29 14:46:38.719079 taskbridge-0.1.2b0/taskbridge/reminders/__init__.py
--rw-r--r--   0        0        0    10528 2024-05-29 14:46:38.719207 taskbridge-0.1.2b0/taskbridge/reminders/controller.py
--rw-r--r--   0        0        0      755 2024-05-29 14:46:38.719402 taskbridge-0.1.2b0/taskbridge/reminders/model/__init__.py
--rw-r--r--   0        0        0    16131 2024-05-29 14:46:38.719609 taskbridge-0.1.2b0/taskbridge/reminders/model/reminder.py
--rw-r--r--   0        0        0    47638 2024-05-29 14:46:38.719843 taskbridge-0.1.2b0/taskbridge/reminders/model/remindercontainer.py
--rw-r--r--   0        0        0     4942 2024-05-29 14:46:38.719972 taskbridge-0.1.2b0/taskbridge/reminders/model/reminderscript.py
--rw-r--r--   0        0        0     9162 1970-01-01 00:00:00.000000 taskbridge-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-05-29 14:46:38.637192 taskbridge-0.1.2b1/LICENSE
+-rw-r--r--   0        0        0     7735 2024-05-29 14:46:38.637482 taskbridge-0.1.2b1/README.md
+-rw-r--r--   0        0        0     1705 2024-05-30 09:29:44.995214 taskbridge-0.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0      348 2024-05-29 14:46:38.665748 taskbridge-0.1.2b1/taskbridge/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-29 14:46:38.665940 taskbridge-0.1.2b1/taskbridge/cli/__init__.py
+-rw-r--r--   0        0        0    19064 2024-05-29 14:46:38.666121 taskbridge-0.1.2b1/taskbridge/cli/tbcli.py
+-rw-r--r--   0        0        0      915 2024-05-29 14:46:38.666360 taskbridge-0.1.2b1/taskbridge/gui/TaskBridge.py
+-rw-r--r--   0        0        0      429 2024-05-29 14:46:38.666525 taskbridge-0.1.2b1/taskbridge/gui/__init__.py
+-rw-r--r--   0        0        0     2846 2024-05-30 09:29:35.964548 taskbridge-0.1.2b1/taskbridge/gui/about.ui
+-rw-r--r--   0        0        0    13473 2024-05-29 14:46:38.667068 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png
+-rw-r--r--   0        0        0    13805 2024-05-29 14:46:38.667348 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png
+-rw-r--r--   0        0        0   772414 2024-05-29 14:46:38.668877 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png
+-rw-r--r--   0        0        0    16622 2024-05-29 14:46:38.671068 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png
+-rw-r--r--   0        0        0    17860 2024-05-29 14:46:38.671293 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png
+-rw-r--r--   0        0        0    19866 2024-05-29 14:46:38.672912 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png
+-rw-r--r--   0        0        0    23814 2024-05-29 14:46:38.673433 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png
+-rw-r--r--   0        0        0    25818 2024-05-29 14:46:38.673746 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png
+-rw-r--r--   0        0        0      822 2024-05-29 14:46:38.674051 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png
+-rw-r--r--   0        0        0    30211 2024-05-29 14:46:38.674423 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png
+-rw-r--r--   0        0        0    31652 2024-05-29 14:46:38.674781 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png
+-rw-r--r--   0        0        0    34032 2024-05-29 14:46:38.675263 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png
+-rw-r--r--   0        0        0    39070 2024-05-29 14:46:38.675737 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png
+-rw-r--r--   0        0        0     1104 2024-05-29 14:46:38.675995 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png
+-rw-r--r--   0        0        0    45736 2024-05-29 14:46:38.676540 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png
+-rw-r--r--   0        0        0    60912 2024-05-29 14:46:38.676837 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png
+-rw-r--r--   0        0        0     1922 2024-05-29 14:46:38.677079 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png
+-rw-r--r--   0        0        0     2235 2024-05-29 14:46:38.677318 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png
+-rw-r--r--   0        0        0     3180 2024-05-29 14:46:38.677584 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png
+-rw-r--r--   0        0        0     4265 2024-05-29 14:46:38.677806 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png
+-rw-r--r--   0        0        0     4543 2024-05-29 14:46:38.678020 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png
+-rw-r--r--   0        0        0   206946 2024-05-29 14:46:38.678816 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png
+-rw-r--r--   0        0        0     5252 2024-05-29 14:46:38.679026 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png
+-rw-r--r--   0        0        0     5549 2024-05-29 14:46:38.679300 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png
+-rw-r--r--   0        0        0     5649 2024-05-29 14:46:38.679428 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png
+-rw-r--r--   0        0        0     5983 2024-05-29 14:46:38.679630 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png
+-rw-r--r--   0        0        0     6583 2024-05-29 14:46:38.679855 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png
+-rw-r--r--   0        0        0     6988 2024-05-29 14:46:38.679989 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png
+-rw-r--r--   0        0        0     7993 2024-05-29 14:46:38.680118 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png
+-rw-r--r--   0        0        0     8732 2024-05-29 14:46:38.680349 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png
+-rw-r--r--   0        0        0     9417 2024-05-29 14:46:38.680628 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png
+-rw-r--r--   0        0        0    10705 2024-05-29 14:46:38.680861 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png
+-rw-r--r--   0        0        0    10894 2024-05-29 14:46:38.680985 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png
+-rw-r--r--   0        0        0    11674 2024-05-29 14:46:38.681115 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png
+-rw-r--r--   0        0        0     7139 2024-05-29 14:46:38.681329 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0        0        0   772414 2024-05-29 14:46:38.681942 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/appstore.png
+-rw-r--r--   0        0        0   214701 2024-05-29 14:46:38.682811 taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/playstore.png
+-rw-r--r--   0        0        0   998221 2024-05-29 14:46:38.685300 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.icns
+-rw-r--r--   0        0        0    17569 2024-05-29 14:46:38.685768 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png
+-rw-r--r--   0        0        0    50656 2024-05-29 14:46:38.686088 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png
+-rw-r--r--   0        0        0     1699 2024-05-29 14:46:38.686298 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png
+-rw-r--r--   0        0        0     2759 2024-05-29 14:46:38.686540 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png
+-rw-r--r--   0        0        0    50655 2024-05-29 14:46:38.686841 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png
+-rw-r--r--   0        0        0   159642 2024-05-29 14:46:38.687387 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png
+-rw-r--r--   0        0        0     2759 2024-05-29 14:46:38.687491 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png
+-rw-r--r--   0        0        0     6510 2024-05-29 14:46:38.689300 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png
+-rw-r--r--   0        0        0   159641 2024-05-29 14:46:38.691223 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png
+-rw-r--r--   0        0        0   551167 2024-05-29 14:46:38.692610 taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png
+-rw-r--r--   0        0        0   931253 2024-05-29 14:46:38.696537 taskbridge-0.1.2b1/taskbridge/gui/assets/source/TaskBridge_Icon.xcf
+-rw-r--r--   0        0        0    69368 2024-05-29 14:46:38.697232 taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge.xcf
+-rw-r--r--   0        0        0   658861 2024-05-29 14:46:38.698526 taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge_animated_black.xcf
+-rw-r--r--   0        0        0    63732 2024-05-29 14:46:38.698922 taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge_animated_optimised.xcf
+-rw-r--r--   0        0        0  1156034 2024-05-29 14:46:38.700882 taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge_animated_white.xcf
+-rw-r--r--   0        0        0   710088 2024-05-29 14:46:38.705680 taskbridge-0.1.2b1/taskbridge/gui/assets/source/dmg_background.png
+-rw-r--r--   0        0        0     3862 2024-05-29 14:46:38.705979 taskbridge-0.1.2b1/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png
+-rw-r--r--   0        0        0     5539 2024-05-29 14:46:38.706230 taskbridge-0.1.2b1/taskbridge/gui/assets/source/ios-swap-7-512.png
+-rw-r--r--   0        0        0     8361 2024-05-29 14:46:38.706503 taskbridge-0.1.2b1/taskbridge/gui/assets/source/local.png
+-rw-r--r--   0        0        0     2197 2024-05-29 14:46:38.706759 taskbridge-0.1.2b1/taskbridge/gui/assets/source/local_and_remote_black.xcf
+-rw-r--r--   0        0        0     3294 2024-05-29 14:46:38.707000 taskbridge-0.1.2b1/taskbridge/gui/assets/source/local_and_remote_white.xcf
+-rw-r--r--   0        0        0    18816 2024-05-29 14:46:38.707358 taskbridge-0.1.2b1/taskbridge/gui/assets/source/remote.png
+-rw-r--r--   0        0        0   825227 2024-05-29 14:46:38.709311 taskbridge-0.1.2b1/taskbridge/gui/assets/source/tb_disk_icon.icns
+-rw-r--r--   0        0        0     1301 2024-05-29 14:46:38.709605 taskbridge-0.1.2b1/taskbridge/gui/assets/table/bidirectional_black.png
+-rw-r--r--   0        0        0     1301 2024-05-29 14:46:38.709828 taskbridge-0.1.2b1/taskbridge/gui/assets/table/bidirectional_white.png
+-rw-r--r--   0        0        0     1591 2024-05-29 14:46:38.710039 taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_and_remote_black.png
+-rw-r--r--   0        0        0     1686 2024-05-29 14:46:38.710255 taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_and_remote_white.png
+-rw-r--r--   0        0        0      965 2024-05-29 14:46:38.710478 taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_black.png
+-rw-r--r--   0        0        0     1950 2024-05-29 14:46:38.710713 taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_to_remote_black.png
+-rw-r--r--   0        0        0     1955 2024-05-29 14:46:38.710919 taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_to_remote_white.png
+-rw-r--r--   0        0        0      990 2024-05-29 14:46:38.711119 taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_white.png
+-rw-r--r--   0        0        0     1266 2024-05-29 14:46:38.711316 taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_black.png
+-rw-r--r--   0        0        0     2885 2024-05-29 14:46:38.711498 taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_to_local_black.png
+-rw-r--r--   0        0        0     2847 2024-05-29 14:46:38.711688 taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_to_local_white.png
+-rw-r--r--   0        0        0     1290 2024-05-29 14:46:38.711895 taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_white.png
+-rw-r--r--   0        0        0    17458 2024-05-29 14:46:38.712296 taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_animated_black.gif
+-rw-r--r--   0        0        0    17522 2024-05-29 14:46:38.712703 taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_animated_white.gif
+-rw-r--r--   0        0        0    47984 2024-05-29 14:46:38.713321 taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_black.png
+-rw-r--r--   0        0        0    11350 2024-05-29 14:46:38.713556 taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_white.png
+-rw-r--r--   0        0        0   387868 2024-05-29 14:46:38.714712 taskbridge-0.1.2b1/taskbridge/gui/assets/ui/TaskBridge.png
+-rw-r--r--   0        0        0     4909 2024-05-29 14:46:38.714953 taskbridge-0.1.2b1/taskbridge/gui/assets/ui/refresh.png
+-rw-r--r--   0        0        0     3701 2024-05-29 14:46:38.715142 taskbridge-0.1.2b1/taskbridge/gui/assets/ui/trash.png
+-rw-r--r--   0        0        0    29304 2024-05-29 19:10:47.968279 taskbridge-0.1.2b1/taskbridge/gui/taskbridge.ui
+-rw-r--r--   0        0        0      908 2024-05-29 14:46:38.715578 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/__init__.py
+-rw-r--r--   0        0        0      476 2024-05-29 14:46:38.715766 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/mainwindow.py
+-rw-r--r--   0        0        0     2703 2024-05-29 14:46:38.715983 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/notecheckbox.py
+-rw-r--r--   0        0        0     1918 2024-05-29 14:46:38.716193 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/remindercheckbox.py
+-rw-r--r--   0        0        0    46116 2024-05-29 14:46:38.716516 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/taskbridgeapp.py
+-rw-r--r--   0        0        0    13063 2024-05-29 14:46:38.716812 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/threadedtasks.py
+-rw-r--r--   0        0        0     1771 2024-05-29 14:46:38.717003 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/trayicon.py
+-rw-r--r--   0        0        0     3201 2024-05-29 14:46:38.717196 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/ui_aboutwindow.py
+-rw-r--r--   0        0        0    33254 2024-05-29 19:13:13.392176 taskbridge-0.1.2b1/taskbridge/gui/viewmodel/ui_mainwindow.py
+-rw-r--r--   0        0        0     5496 2024-05-29 14:46:38.717636 taskbridge-0.1.2b1/taskbridge/helpers.py
+-rw-r--r--   0        0        0      570 2024-05-29 14:46:38.717839 taskbridge-0.1.2b1/taskbridge/notes/__init__.py
+-rw-r--r--   0        0        0     7391 2024-05-29 14:46:38.718013 taskbridge-0.1.2b1/taskbridge/notes/controller.py
+-rw-r--r--   0        0        0      572 2024-05-29 14:46:38.718265 taskbridge-0.1.2b1/taskbridge/notes/model/__init__.py
+-rw-r--r--   0        0        0    19383 2024-05-29 14:46:38.718466 taskbridge-0.1.2b1/taskbridge/notes/model/note.py
+-rw-r--r--   0        0        0    44186 2024-05-29 19:06:11.452492 taskbridge-0.1.2b1/taskbridge/notes/model/notefolder.py
+-rw-r--r--   0        0        0     6063 2024-05-29 14:46:38.718887 taskbridge-0.1.2b1/taskbridge/notes/model/notescript.py
+-rw-r--r--   0        0        0      651 2024-05-29 14:46:38.719079 taskbridge-0.1.2b1/taskbridge/reminders/__init__.py
+-rw-r--r--   0        0        0    10528 2024-05-29 14:46:38.719207 taskbridge-0.1.2b1/taskbridge/reminders/controller.py
+-rw-r--r--   0        0        0      755 2024-05-29 14:46:38.719402 taskbridge-0.1.2b1/taskbridge/reminders/model/__init__.py
+-rw-r--r--   0        0        0    16131 2024-05-29 14:46:38.719609 taskbridge-0.1.2b1/taskbridge/reminders/model/reminder.py
+-rw-r--r--   0        0        0    47638 2024-05-29 14:46:38.719843 taskbridge-0.1.2b1/taskbridge/reminders/model/remindercontainer.py
+-rw-r--r--   0        0        0     4942 2024-05-29 14:46:38.719972 taskbridge-0.1.2b1/taskbridge/reminders/model/reminderscript.py
+-rw-r--r--   0        0        0     9162 1970-01-01 00:00:00.000000 taskbridge-0.1.2b1/PKG-INFO
```

### Comparing `taskbridge-0.1.2b0/LICENSE` & `taskbridge-0.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/README.md` & `taskbridge-0.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/pyproject.toml` & `taskbridge-0.1.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TaskBridge"
-version = "0.1.2-beta"
+version = "0.1.2-beta.1"
 description = "Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!"
 keywords = ["sync", "note sync", "reminder sync", "cloud notes", "cloud reminders"]
 authors = ["Pint-Sized Software <hello@pintsized.dev>"]
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
```

### Comparing `taskbridge-0.1.2b0/taskbridge/cli/tbcli.py` & `taskbridge-0.1.2b1/taskbridge/cli/tbcli.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/TaskBridge.py` & `taskbridge-0.1.2b1/taskbridge/gui/TaskBridge.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/about.ui` & `taskbridge-0.1.2b1/taskbridge/gui/about.ui`

 * *Files 0% similar despite different names*

#### Comparing `taskbridge-0.1.2b0/taskbridge/gui/about.ui` & `taskbridge-0.1.2b1/taskbridge/gui/about.ui`

```diff
@@ -89,15 +89,15 @@
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="lbl_version">
           <property name="text">
-            <string>Version 0.1.2-beta</string>
+            <string>Version 0.1.2-beta.1</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
```

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/appstore.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/appstore.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/playstore.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/AppIcons/playstore.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.icns` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.icns`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/TaskBridge_Icon.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/TaskBridge_Icon.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_black.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge_animated_black.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_optimised.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge_animated_optimised.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_white.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/bridge_animated_white.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/dmg_background.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/dmg_background.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-swap-7-512.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/ios-swap-7-512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/local.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/local.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_black.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/local_and_remote_black.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_white.xcf` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/local_and_remote_white.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/remote.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/remote.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/source/tb_disk_icon.icns` & `taskbridge-0.1.2b1/taskbridge/gui/assets/source/tb_disk_icon.icns`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/bidirectional_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/bidirectional_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_and_remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_and_remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_to_remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_to_remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/local_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_to_local_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_to_local_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/table/remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_black.gif` & `taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_animated_black.gif`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_white.gif` & `taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_animated_white.gif`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_black.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_white.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/tray/bridge_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/ui/TaskBridge.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/ui/TaskBridge.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/ui/refresh.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/ui/refresh.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/assets/ui/trash.png` & `taskbridge-0.1.2b1/taskbridge/gui/assets/ui/trash.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/taskbridge.ui` & `taskbridge-0.1.2b1/taskbridge/gui/taskbridge.ui`

 * *Files 0% similar despite different names*

#### Comparing `taskbridge-0.1.2b0/taskbridge/gui/taskbridge.ui` & `taskbridge-0.1.2b1/taskbridge/gui/taskbridge.ui`

```diff
@@ -20,15 +20,15 @@
       <string>TaskBridge</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QVBoxLayout" name="verticalLayout">
         <item alignment="Qt::AlignTop">
           <widget class="QTabWidget" name="tab_container">
             <property name="currentIndex">
-              <number>2</number>
+              <number>0</number>
             </property>
             <widget class="QWidget" name="tab_sync">
               <attribute name="title">
                 <string>Sync</string>
               </attribute>
               <layout class="QVBoxLayout" name="verticalLayout_7">
                 <item>
@@ -144,14 +144,16 @@
                                     <bool>true</bool>
                                   </property>
                                   <property name="html">
                                     <string>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
 &lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;meta charset=&quot;utf-8&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
 p, li { white-space: pre-wrap; }
 hr { height: 1px; border-width: 0; }
+li.unchecked::marker { content: &quot;\2610&quot;; }
+li.checked::marker { content: &quot;\2612&quot;; }
 &lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'.AppleSystemUIFont'; font-size:13pt; font-weight:400; font-style:normal;&quot;&gt;
 &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-weight:700;&quot;&gt;TaskBridge Initialised&lt;/span&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
                                   </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
@@ -233,14 +235,17 @@
                               </property>
                               <property name="minimumSize">
                                 <size>
                                   <width>50</width>
                                   <height>0</height>
                                 </size>
                               </property>
+                              <property name="value">
+                                <number>10</number>
+                              </property>
                             </widget>
                           </item>
                           <item>
                             <widget class="QComboBox" name="cmb_sync_frequency">
                               <item>
                                 <property name="text">
                                   <string>Minutes</string>
```

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/__init__.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/notecheckbox.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/notecheckbox.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/remindercheckbox.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/remindercheckbox.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/taskbridgeapp.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/taskbridgeapp.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/threadedtasks.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/threadedtasks.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/trayicon.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/trayicon.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_aboutwindow.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/ui_aboutwindow.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_mainwindow.py` & `taskbridge-0.1.2b1/taskbridge/gui/viewmodel/ui_mainwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Form implementation generated from reading ui file 'taskbridge.ui'
+# Form implementation generated from reading ui file 'taskBridge.ui'
 #
-# Created by: PyQt6 UI code generator 6.6.1
+# Created by: PyQt6 UI code generator 6.7.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
@@ -120,14 +120,15 @@
         self.spn_sync_frequency = QtWidgets.QSpinBox(parent=self.gb_autosync)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.spn_sync_frequency.sizePolicy().hasHeightForWidth())
         self.spn_sync_frequency.setSizePolicy(sizePolicy)
         self.spn_sync_frequency.setMinimumSize(QtCore.QSize(50, 0))
+        self.spn_sync_frequency.setProperty("value", 10)
         self.spn_sync_frequency.setObjectName("spn_sync_frequency")
         self.horizontalLayout_3.addWidget(self.spn_sync_frequency)
         self.cmb_sync_frequency = QtWidgets.QComboBox(parent=self.gb_autosync)
         self.cmb_sync_frequency.setObjectName("cmb_sync_frequency")
         self.cmb_sync_frequency.addItem("")
         self.cmb_sync_frequency.addItem("")
         self.horizontalLayout_3.addWidget(self.cmb_sync_frequency)
@@ -391,15 +392,15 @@
         self.menuView.addSeparator()
         self.menuTaskBridge.addAction(self.actionQuit_TaskBridge)
         self.menubar.addAction(self.menuView.menuAction())
         self.menubar.addAction(self.menuHelp.menuAction())
         self.menubar.addAction(self.menuTaskBridge.menuAction())
 
         self.retranslateUi(MainWindow)
-        self.tab_container.setCurrentIndex(2)
+        self.tab_container.setCurrentIndex(0)
         self.stackedWidget.setCurrentIndex(0)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
         MainWindow.setTabOrder(self.tab_container, self.btn_sync)
         MainWindow.setTabOrder(self.btn_sync, self.btn_sync_view)
         MainWindow.setTabOrder(self.btn_sync_view, self.cb_sync_scheduled)
         MainWindow.setTabOrder(self.cb_sync_scheduled, self.spn_sync_frequency)
         MainWindow.setTabOrder(self.spn_sync_frequency, self.cmb_sync_frequency)
@@ -433,14 +434,16 @@
         self.cmb_sync_log_level.setItemText(1, _translate("MainWindow", "Info"))
         self.cmb_sync_log_level.setItemText(2, _translate("MainWindow", "Debug"))
         self.btn_clear_logs.setText(_translate("MainWindow", "..."))
         self.txt_log_display.setHtml(_translate("MainWindow", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
 "<html><head><meta name=\"qrichtext\" content=\"1\" /><meta charset=\"utf-8\" /><style type=\"text/css\">\n"
 "p, li { white-space: pre-wrap; }\n"
 "hr { height: 1px; border-width: 0; }\n"
+"li.unchecked::marker { content: \"\\2610\"; }\n"
+"li.checked::marker { content: \"\\2612\"; }\n"
 "</style></head><body style=\" font-family:\'.AppleSystemUIFont\'; font-size:13pt; font-weight:400; font-style:normal;\">\n"
 "<p style=\" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><span style=\" font-weight:700;\">TaskBridge Initialised</span></p></body></html>"))
         self.btn_sync.setText(_translate("MainWindow", "Sync"))
         self.btn_sync_view.setText(_translate("MainWindow", "..."))
         self.lbl_sync_status.setText(_translate("MainWindow", "Currently Idle."))
         self.cb_sync_scheduled.setText(_translate("MainWindow", "Scheduled Sync"))
         self.label_4.setText(_translate("MainWindow", "Synchronise every"))
@@ -494,7 +497,17 @@
         self.actionOink.setText(_translate("MainWindow", "Oink"))
         self.actionDocumentation.setText(_translate("MainWindow", "Documentation"))
         self.actionAbout_TaskBridge.setText(_translate("MainWindow", "About TaskBridge"))
         self.actionSync.setText(_translate("MainWindow", "Sync"))
         self.actionReminders.setText(_translate("MainWindow", "Reminders"))
         self.actionNotes.setText(_translate("MainWindow", "Notes"))
         self.actionQuit_TaskBridge.setText(_translate("MainWindow", "Quit TaskBridge"))
+
+
+if __name__ == "__main__":
+    import sys
+    app = QtWidgets.QApplication(sys.argv)
+    MainWindow = QtWidgets.QMainWindow()
+    ui = Ui_MainWindow()
+    ui.setupUi(MainWindow)
+    MainWindow.show()
+    sys.exit(app.exec())
```

### Comparing `taskbridge-0.1.2b0/taskbridge/helpers.py` & `taskbridge-0.1.2b1/taskbridge/helpers.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/notes/__init__.py` & `taskbridge-0.1.2b1/taskbridge/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/notes/controller.py` & `taskbridge-0.1.2b1/taskbridge/notes/controller.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/notes/model/__init__.py` & `taskbridge-0.1.2b1/taskbridge/notes/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/notes/model/note.py` & `taskbridge-0.1.2b1/taskbridge/notes/model/note.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/notes/model/notefolder.py` & `taskbridge-0.1.2b1/taskbridge/notes/model/notefolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Contains the ``NoteFolder`` class, which represents a folder containing notes, either locally or remotely.
 Many of the synchronisation methods are here.
 """
 
 from __future__ import annotations
 
 import copy
+import datetime
 import glob
 import os
 import shutil
 import sqlite3
 from contextlib import closing
 from pathlib import Path
 from typing import List
@@ -74,14 +75,15 @@
         :returns:
 
             -success (:py:class:`bool`) - true if notes are successfully loaded.
 
             -data (:py:class:`str` | :py:class:`int`) - error message on failure, or number of notes loaded on success.
 
         """
+        self.local_notes.clear()
         get_notes_script = notescript.get_notes_script
         return_code, stdout, stderr = helpers.run_applescript(get_notes_script, self.local_folder.name)
 
         if return_code != 0:
             return False, stderr
 
         staging_folder_path = stdout.strip()
@@ -108,14 +110,16 @@
         :returns:
 
             -success (:py:class:`bool`) - true if notes are successfully loaded.
 
             -data (:py:class:`str` | :py:class:`int`) - error message on failure, or number of notes loaded on success.
 
         """
+        self.remote_notes.clear()
+
         for root, dirs, files in os.walk(self.remote_folder.path):
             for remote_file in files:
                 f_name, f_ext = os.path.splitext(remote_file)
                 if not f_ext == ".md":
                     continue
                 remote_note = self.remote_folder.path / remote_file
                 with open(remote_note) as fp:
@@ -149,14 +153,16 @@
                 result[key].append(remote.name)
                 return True, i_data
         return True, ''
 
     def sync_remote_note_to_local(self, local: Note, remote: Note, result: dict) -> tuple[bool, str]:
         """
         Sync remote notes to local. This performs an update or an insert.
+        Since the Apple Notes modified date is read only, we have to update the modified date of the remote note as well,
+        otherwise the remote note will be overwritten on the next sync.
 
         :param local: the local note.
         :param remote: the remote note.
         :param result: a dictionary where results of sync will be saved.
 
         :returns:
 
@@ -169,14 +175,19 @@
             key = 'local_updated'
             local = copy.deepcopy(remote)
             if helpers.confirm("Update local note {}".format(local.name)):
                 i_success, i_data = local.update_local(self.local_folder.name)
                 if not i_success:
                     return False, i_data
                 result[key].append(local.name)
+
+                # Update modification date of remote note
+                remote.modified_date = datetime.datetime.now()
+                remote.upsert_remote(self.remote_folder.path)
+
                 return True, i_data
         return True, 'Sync skipped since local note has been modified.'
 
     def sync_local_to_remote(self, result: dict) -> tuple[bool, str]:
         """
         Sync all the local notes in this folder to remote.
```

### Comparing `taskbridge-0.1.2b0/taskbridge/notes/model/notescript.py` & `taskbridge-0.1.2b1/taskbridge/notes/model/notescript.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/reminders/__init__.py` & `taskbridge-0.1.2b1/taskbridge/reminders/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/reminders/controller.py` & `taskbridge-0.1.2b1/taskbridge/reminders/controller.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/reminders/model/__init__.py` & `taskbridge-0.1.2b1/taskbridge/reminders/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/reminders/model/reminder.py` & `taskbridge-0.1.2b1/taskbridge/reminders/model/reminder.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/reminders/model/remindercontainer.py` & `taskbridge-0.1.2b1/taskbridge/reminders/model/remindercontainer.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/taskbridge/reminders/model/reminderscript.py` & `taskbridge-0.1.2b1/taskbridge/reminders/model/reminderscript.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.2b0/PKG-INFO` & `taskbridge-0.1.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaskBridge
-Version: 0.1.2b0
+Version: 0.1.2b1
 Summary: Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!
 Home-page: https://taskbridge.app/
 License: GPL-3.0-or-later
 Keywords: sync,note sync,reminder sync,cloud notes,cloud reminders
 Author: Pint-Sized Software
 Author-email: hello@pintsized.dev
 Requires-Python: >=3.10,<3.13
```

