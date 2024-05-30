# Comparing `tmp/sticker_convert-2.8.8.tar.gz` & `tmp/sticker_convert-2.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sticker_convert-2.8.8.tar", last modified: Wed May 22 08:36:03 2024, max compression
+gzip compressed data, was "sticker_convert-2.8.9.tar", last modified: Thu May 23 13:53:53 2024, max compression
```

## Comparing `sticker_convert-2.8.8.tar` & `sticker_convert-2.8.9.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.890105 sticker_convert-2.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-05-22 08:36:03.890105 sticker_convert-2.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:36:03.890105 sticker_convert-2.8.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.866105 sticker_convert-2.8.8/src/sticker_convert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18621 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37357 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.866105 sticker_convert-2.8.8/src/sticker_convert/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_line.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/downloaders/download_viber.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30707 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.866105 sticker_convert-2.8.8/src/sticker_convert/gui_components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/comp_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/config_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/control_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/cred_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/input_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/output_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/progress_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/right_clicker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/gui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31964 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/advanced_compression_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/base_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/line_get_auth_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.870105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
--rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.862105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.874105 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
--rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7732 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/job_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/resources/
--rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/NotoColorEmoji.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/appicon.icns
--rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/appicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/appicon.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    12156 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/compression.json
--rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/emoji.json
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/help.json
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/input.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/resources/output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/uploaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/compress_wastickers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_telegram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/uploaders/xcode_imessage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_kakao_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_line_auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_signal_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/files/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/cache_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/json_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/json_resources_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10100 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/metadata_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/run_bin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/files/sanitize_filename.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert/utils/media/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/apple_png_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/codec_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/decrypt_kakao.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/media/format_verify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/utils/url_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/src/sticker_convert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/src/sticker_convert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50061 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 08:36:03.000000 sticker_convert-2.8.8/src/sticker_convert.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:36:03.886105 sticker_convert-2.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-22 08:35:56.000000 sticker_convert-2.8.8/tests/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    50350 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27854 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.557539 sticker_convert-2.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.561539 sticker_convert-2.8.9/src/sticker_convert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      102 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19020 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38099 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.561539 sticker_convert-2.8.9/src/sticker_convert/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/download_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8516 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/download_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17853 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/download_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/download_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4614 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/download_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/downloaders/download_viber.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30806 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/gui_components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/comp_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/config_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/control_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/cred_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/input_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/output_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/progress_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/right_clicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/gui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32675 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/advanced_compression_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/base_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/line_get_auth_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/signal_get_auth_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.565539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.557539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/
+-rw-r--r--   0 runner    (1001) docker     (127)    21835 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.557539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.557539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.569539 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/xcuserdata/niklaspeterson.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25775 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7772 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/job_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.581539 sticker_convert-2.8.9/src/sticker_convert/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (127) 10353636 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/NotoColorEmoji.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5404 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/appicon.icns
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38078 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/appicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/appicon.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12528 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/compression.json
+-rw-r--r--   0 runner    (1001) docker     (127)   413367 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/emoji.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/help.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/resources/output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.581539 sticker_convert-2.8.9/src/sticker_convert/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/uploaders/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6021 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/uploaders/compress_wastickers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1203 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/uploaders/upload_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6396 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/uploaders/upload_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15695 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/uploaders/upload_telegram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11254 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/uploaders/xcode_imessage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.581539 sticker_convert-2.8.9/src/sticker_convert/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.581539 sticker_convert-2.8.9/src/sticker_convert/utils/auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9829 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/auth/get_kakao_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/auth/get_line_auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4925 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/auth/get_signal_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/src/sticker_convert/utils/files/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/files/cache_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/files/json_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/files/json_resources_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10100 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/files/metadata_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1743 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/files/run_bin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2156 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/files/sanitize_filename.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/src/sticker_convert/utils/media/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3657 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/media/apple_png_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/media/codec_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/media/decrypt_kakao.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5732 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/media/format_verify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      840 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/utils/url_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 13:53:46.000000 sticker_convert-2.8.9/src/sticker_convert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/src/sticker_convert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50350 2024-05-23 13:53:53.000000 sticker_convert-2.8.9/src/sticker_convert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-23 13:53:53.000000 sticker_convert-2.8.9/src/sticker_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:53:53.000000 sticker_convert-2.8.9/src/sticker_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 13:53:53.000000 sticker_convert-2.8.9/src/sticker_convert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 13:53:53.000000 sticker_convert-2.8.9/src/sticker_convert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 13:53:53.000000 sticker_convert-2.8.9/src/sticker_convert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:53:53.585539 sticker_convert-2.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-23 13:53:47.000000 sticker_convert-2.8.9/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-05-23 13:53:47.000000 sticker_convert-2.8.9/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-23 13:53:47.000000 sticker_convert-2.8.9/tests/test_export.py
```

### Comparing `sticker_convert-2.8.8/LICENSE` & `sticker_convert-2.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/PKG-INFO` & `sticker_convert-2.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.8
+Version: 2.8.9
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -475,44 +475,49 @@
 7. Enter credentials if you want to download/upload from telegram or upload from Signal (View 'Compatability' and 'FAQ' section for more information)
 8. Press 'Start'
 
 ## How to use (CLI)
 To run in CLI mode, pass on any arguments
 
 ```
-usage: sticker-convert.py [-h] [--version] [--no-confirm] [--custom-presets CUSTOM_PRESETS] [--input-dir INPUT_DIR]
+usage: sticker-convert.py [-h] [--version] [--no-confirm] [--no-progress] [--custom-presets CUSTOM_PRESETS] [--input-dir INPUT_DIR]
                           [--download-auto DOWNLOAD_AUTO | --download-signal DOWNLOAD_SIGNAL | --download-telegram DOWNLOAD_TELEGRAM | --download-line DOWNLOAD_LINE | --download-kakao DOWNLOAD_KAKAO | --download-viber DOWNLOAD_VIBER]
-                          [--output-dir OUTPUT_DIR] [--author AUTHOR] [--title TITLE] [--export-signal | --export-telegram | --export-telegram-emoji | --export-whatsapp | --export-imessage]
-                          [--no-compress] [--preset {auto,signal,telegram,telegram_emoji,whatsapp,line,kakao,viber,imessage_small,imessage_medium,imessage_large,custom}] [--steps STEPS]
-                          [--processes PROCESSES] [--fps-min FPS_MIN] [--fps-max FPS_MAX] [--fps-power FPS_POWER] [--res-min RES_MIN] [--res-max RES_MAX] [--res-w-min RES_W_MIN] [--res-w-max RES_W_MAX]
-                          [--res-h-min RES_H_MIN] [--res-h-max RES_H_MAX] [--res-power RES_POWER] [--quality-min QUALITY_MIN] [--quality-max QUALITY_MAX] [--quality-power QUALITY_POWER]
-                          [--color-min COLOR_MIN] [--color-max COLOR_MAX] [--color-power COLOR_POWER] [--duration-min DURATION_MIN] [--duration-max DURATION_MAX] [--padding-percent PADDING_PERCENT]
-                          [--bg-color BG_COLOR] [--vid-size-max VID_SIZE_MAX] [--img-size-max IMG_SIZE_MAX] [--vid-format VID_FORMAT] [--img-format IMG_FORMAT] [--fake-vid] [--scale-filter SCALE_FILTER]
-                          [--quantize-method QUANTIZE_METHOD] [--cache-dir CACHE_DIR] [--default-emoji DEFAULT_EMOJI] [--signal-uuid SIGNAL_UUID] [--signal-password SIGNAL_PASSWORD] [--signal-get-auth]
-                          [--signal-data-dir SIGNAL_DATA_DIR] [--telegram-token TELEGRAM_TOKEN] [--telegram-userid TELEGRAM_USERID] [--kakao-auth-token KAKAO_AUTH_TOKEN] [--kakao-get-auth]
-                          [--kakao-username KAKAO_USERNAME] [--kakao-password KAKAO_PASSWORD] [--kakao-country-code KAKAO_COUNTRY_CODE] [--kakao-phone-number KAKAO_PHONE_NUMBER] [--line-get-auth]
-                          [--line-cookies LINE_COOKIES] [--save-cred SAVE_CRED]
+                          [--output-dir OUTPUT_DIR] [--author AUTHOR] [--title TITLE]
+                          [--export-signal | --export-telegram | --export-telegram-emoji | --export-whatsapp | --export-imessage] [--no-compress]
+                          [--preset {auto,signal,telegram,telegram_emoji,whatsapp,line,kakao,viber,imessage_small,imessage_medium,imessage_large,custom}]
+                          [--steps STEPS] [--processes PROCESSES] [--fps-min FPS_MIN] [--fps-max FPS_MAX] [--fps-power FPS_POWER] [--res-min RES_MIN]
+                          [--res-max RES_MAX] [--res-w-min RES_W_MIN] [--res-w-max RES_W_MAX] [--res-h-min RES_H_MIN] [--res-h-max RES_H_MAX]
+                          [--res-power RES_POWER] [--quality-min QUALITY_MIN] [--quality-max QUALITY_MAX] [--quality-power QUALITY_POWER] [--color-min COLOR_MIN]
+                          [--color-max COLOR_MAX] [--color-power COLOR_POWER] [--duration-min DURATION_MIN] [--duration-max DURATION_MAX]
+                          [--padding-percent PADDING_PERCENT] [--bg-color BG_COLOR] [--vid-size-max VID_SIZE_MAX] [--img-size-max IMG_SIZE_MAX]
+                          [--vid-format VID_FORMAT] [--img-format IMG_FORMAT] [--fake-vid] [--scale-filter SCALE_FILTER] [--quantize-method QUANTIZE_METHOD]
+                          [--force-pywebp] [--cache-dir CACHE_DIR] [--default-emoji DEFAULT_EMOJI] [--signal-uuid SIGNAL_UUID] [--signal-password SIGNAL_PASSWORD]
+                          [--signal-get-auth] [--signal-data-dir SIGNAL_DATA_DIR] [--telegram-token TELEGRAM_TOKEN] [--telegram-userid TELEGRAM_USERID]
+                          [--kakao-auth-token KAKAO_AUTH_TOKEN] [--kakao-get-auth] [--kakao-username KAKAO_USERNAME] [--kakao-password KAKAO_PASSWORD]
+                          [--kakao-country-code KAKAO_COUNTRY_CODE] [--kakao-phone-number KAKAO_PHONE_NUMBER] [--line-get-auth] [--line-cookies LINE_COOKIES]
+                          [--save-cred SAVE_CRED]
 
 CLI for stickers-convert
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   --no-confirm          Do not ask any questions.
+  --no-progress         Do not show progress bar in CLI.
   --custom-presets CUSTOM_PRESETS
                         Specify a json file containing custom compression presets.
                         See compression.json for format.
                         Note that if present, 'custom_preset.json' from config directory would be auto loaded.
 
 Input options:
   --input-dir INPUT_DIR
                         Specify input directory.
   --download-auto DOWNLOAD_AUTO
                         Auto detect URL type and download
-                        (Supported input sources: Signal, Telegram, Line, Kakao)
+                        (Supported input sources: Signal, Telegram, Line, Kakao, Viber)
   --download-signal DOWNLOAD_SIGNAL
                         Download signal stickers from a URL as input
                         (Example: https://signal.art/addstickers/#pack_id=xxxxx&pack_key=xxxxx)
   --download-telegram DOWNLOAD_TELEGRAM
                         Download telegram stickers from a URL as input
                         (Example: https://telegram.me/addstickers/xxxxx
                          OR https://telegram.me/addemoji/xxxxx)
@@ -583,15 +588,15 @@
   --duration-min DURATION_MIN
                         Set minimum output duration in miliseconds.
   --duration-max DURATION_MAX
                         Set maximum output duration in miliseconds.
   --padding-percent PADDING_PERCENT
                         Set percentage of space used as padding.
   --bg-color BG_COLOR   Set custom background color in rrggbbaa format.
-                        Example: 00ff00 for green with alpha 0.
+                        Example: 00ff0000 for green with alpha 0.
                         If this is not set, background color would be auto set to black if image is bright, or white if image is dark.
                         Note: The color should not be visible if output format supports transparency.
   --vid-size-max VID_SIZE_MAX
                         Set maximum file size limit for animated stickers.
   --img-size-max IMG_SIZE_MAX
                         Set maximum file size limit for static stickers.
   --vid-format VID_FORMAT
@@ -611,14 +616,15 @@
                         - bicubic = Cubic spline interpolation
                         - lanczos = A high-quality downsampling filter
   --quantize-method QUANTIZE_METHOD
                         Set method for quantizing image. Default as imagequant. Valid options are:
                         - imagequant = Best quality but slow
                         - fastoctree = Fast but image looks chunky
                         - none = No image quantizing, large image size as result
+  --force-pywebp        Force using pywebp for encoding webp files instead of Pillow.
   --cache-dir CACHE_DIR
                         Set custom cache directory.
                         Useful for debugging, or speed up conversion if cache_dir is on RAM disk.
   --default-emoji DEFAULT_EMOJI
                         Set the default emoji for uploading Signal and Telegram sticker packs.
 
 Credentials options:
```

### Comparing `sticker_convert-2.8.8/README.md` & `sticker_convert-2.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,44 +88,49 @@
 7. Enter credentials if you want to download/upload from telegram or upload from Signal (View 'Compatability' and 'FAQ' section for more information)
 8. Press 'Start'
 
 ## How to use (CLI)
 To run in CLI mode, pass on any arguments
 
 ```
-usage: sticker-convert.py [-h] [--version] [--no-confirm] [--custom-presets CUSTOM_PRESETS] [--input-dir INPUT_DIR]
+usage: sticker-convert.py [-h] [--version] [--no-confirm] [--no-progress] [--custom-presets CUSTOM_PRESETS] [--input-dir INPUT_DIR]
                           [--download-auto DOWNLOAD_AUTO | --download-signal DOWNLOAD_SIGNAL | --download-telegram DOWNLOAD_TELEGRAM | --download-line DOWNLOAD_LINE | --download-kakao DOWNLOAD_KAKAO | --download-viber DOWNLOAD_VIBER]
-                          [--output-dir OUTPUT_DIR] [--author AUTHOR] [--title TITLE] [--export-signal | --export-telegram | --export-telegram-emoji | --export-whatsapp | --export-imessage]
-                          [--no-compress] [--preset {auto,signal,telegram,telegram_emoji,whatsapp,line,kakao,viber,imessage_small,imessage_medium,imessage_large,custom}] [--steps STEPS]
-                          [--processes PROCESSES] [--fps-min FPS_MIN] [--fps-max FPS_MAX] [--fps-power FPS_POWER] [--res-min RES_MIN] [--res-max RES_MAX] [--res-w-min RES_W_MIN] [--res-w-max RES_W_MAX]
-                          [--res-h-min RES_H_MIN] [--res-h-max RES_H_MAX] [--res-power RES_POWER] [--quality-min QUALITY_MIN] [--quality-max QUALITY_MAX] [--quality-power QUALITY_POWER]
-                          [--color-min COLOR_MIN] [--color-max COLOR_MAX] [--color-power COLOR_POWER] [--duration-min DURATION_MIN] [--duration-max DURATION_MAX] [--padding-percent PADDING_PERCENT]
-                          [--bg-color BG_COLOR] [--vid-size-max VID_SIZE_MAX] [--img-size-max IMG_SIZE_MAX] [--vid-format VID_FORMAT] [--img-format IMG_FORMAT] [--fake-vid] [--scale-filter SCALE_FILTER]
-                          [--quantize-method QUANTIZE_METHOD] [--cache-dir CACHE_DIR] [--default-emoji DEFAULT_EMOJI] [--signal-uuid SIGNAL_UUID] [--signal-password SIGNAL_PASSWORD] [--signal-get-auth]
-                          [--signal-data-dir SIGNAL_DATA_DIR] [--telegram-token TELEGRAM_TOKEN] [--telegram-userid TELEGRAM_USERID] [--kakao-auth-token KAKAO_AUTH_TOKEN] [--kakao-get-auth]
-                          [--kakao-username KAKAO_USERNAME] [--kakao-password KAKAO_PASSWORD] [--kakao-country-code KAKAO_COUNTRY_CODE] [--kakao-phone-number KAKAO_PHONE_NUMBER] [--line-get-auth]
-                          [--line-cookies LINE_COOKIES] [--save-cred SAVE_CRED]
+                          [--output-dir OUTPUT_DIR] [--author AUTHOR] [--title TITLE]
+                          [--export-signal | --export-telegram | --export-telegram-emoji | --export-whatsapp | --export-imessage] [--no-compress]
+                          [--preset {auto,signal,telegram,telegram_emoji,whatsapp,line,kakao,viber,imessage_small,imessage_medium,imessage_large,custom}]
+                          [--steps STEPS] [--processes PROCESSES] [--fps-min FPS_MIN] [--fps-max FPS_MAX] [--fps-power FPS_POWER] [--res-min RES_MIN]
+                          [--res-max RES_MAX] [--res-w-min RES_W_MIN] [--res-w-max RES_W_MAX] [--res-h-min RES_H_MIN] [--res-h-max RES_H_MAX]
+                          [--res-power RES_POWER] [--quality-min QUALITY_MIN] [--quality-max QUALITY_MAX] [--quality-power QUALITY_POWER] [--color-min COLOR_MIN]
+                          [--color-max COLOR_MAX] [--color-power COLOR_POWER] [--duration-min DURATION_MIN] [--duration-max DURATION_MAX]
+                          [--padding-percent PADDING_PERCENT] [--bg-color BG_COLOR] [--vid-size-max VID_SIZE_MAX] [--img-size-max IMG_SIZE_MAX]
+                          [--vid-format VID_FORMAT] [--img-format IMG_FORMAT] [--fake-vid] [--scale-filter SCALE_FILTER] [--quantize-method QUANTIZE_METHOD]
+                          [--force-pywebp] [--cache-dir CACHE_DIR] [--default-emoji DEFAULT_EMOJI] [--signal-uuid SIGNAL_UUID] [--signal-password SIGNAL_PASSWORD]
+                          [--signal-get-auth] [--signal-data-dir SIGNAL_DATA_DIR] [--telegram-token TELEGRAM_TOKEN] [--telegram-userid TELEGRAM_USERID]
+                          [--kakao-auth-token KAKAO_AUTH_TOKEN] [--kakao-get-auth] [--kakao-username KAKAO_USERNAME] [--kakao-password KAKAO_PASSWORD]
+                          [--kakao-country-code KAKAO_COUNTRY_CODE] [--kakao-phone-number KAKAO_PHONE_NUMBER] [--line-get-auth] [--line-cookies LINE_COOKIES]
+                          [--save-cred SAVE_CRED]
 
 CLI for stickers-convert
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   --no-confirm          Do not ask any questions.
+  --no-progress         Do not show progress bar in CLI.
   --custom-presets CUSTOM_PRESETS
                         Specify a json file containing custom compression presets.
                         See compression.json for format.
                         Note that if present, 'custom_preset.json' from config directory would be auto loaded.
 
 Input options:
   --input-dir INPUT_DIR
                         Specify input directory.
   --download-auto DOWNLOAD_AUTO
                         Auto detect URL type and download
-                        (Supported input sources: Signal, Telegram, Line, Kakao)
+                        (Supported input sources: Signal, Telegram, Line, Kakao, Viber)
   --download-signal DOWNLOAD_SIGNAL
                         Download signal stickers from a URL as input
                         (Example: https://signal.art/addstickers/#pack_id=xxxxx&pack_key=xxxxx)
   --download-telegram DOWNLOAD_TELEGRAM
                         Download telegram stickers from a URL as input
                         (Example: https://telegram.me/addstickers/xxxxx
                          OR https://telegram.me/addemoji/xxxxx)
@@ -196,15 +201,15 @@
   --duration-min DURATION_MIN
                         Set minimum output duration in miliseconds.
   --duration-max DURATION_MAX
                         Set maximum output duration in miliseconds.
   --padding-percent PADDING_PERCENT
                         Set percentage of space used as padding.
   --bg-color BG_COLOR   Set custom background color in rrggbbaa format.
-                        Example: 00ff00 for green with alpha 0.
+                        Example: 00ff0000 for green with alpha 0.
                         If this is not set, background color would be auto set to black if image is bright, or white if image is dark.
                         Note: The color should not be visible if output format supports transparency.
   --vid-size-max VID_SIZE_MAX
                         Set maximum file size limit for animated stickers.
   --img-size-max IMG_SIZE_MAX
                         Set maximum file size limit for static stickers.
   --vid-format VID_FORMAT
@@ -224,14 +229,15 @@
                         - bicubic = Cubic spline interpolation
                         - lanczos = A high-quality downsampling filter
   --quantize-method QUANTIZE_METHOD
                         Set method for quantizing image. Default as imagequant. Valid options are:
                         - imagequant = Best quality but slow
                         - fastoctree = Fast but image looks chunky
                         - none = No image quantizing, large image size as result
+  --force-pywebp        Force using pywebp for encoding webp files instead of Pillow.
   --cache-dir CACHE_DIR
                         Set custom cache directory.
                         Useful for debugging, or speed up conversion if cache_dir is on RAM disk.
   --default-emoji DEFAULT_EMOJI
                         Set the default emoji for uploading Signal and Telegram sticker packs.
 
 Credentials options:
```

### Comparing `sticker_convert-2.8.8/pyproject.toml` & `sticker_convert-2.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/cli.py` & `sticker_convert-2.8.9/src/sticker_convert/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,20 @@
         parser.add_argument(
             "--no-confirm",
             dest="no_confirm",
             action="store_true",
             help=self.help["global"]["no_confirm"],
         )
         parser.add_argument(
+            "--no-progress",
+            dest="no_progress",
+            action="store_true",
+            help=self.help["global"]["no_progress"],
+        )
+        parser.add_argument(
             "--custom-presets",
             dest="custom_presets",
             default=None,
             help=self.help["global"]["custom_presets"],
         )
 
         parser_input = parser.add_argument_group("Input options")
@@ -126,15 +132,15 @@
             "bg_color",
             "vid_format",
             "img_format",
             "cache_dir",
             "scale_filter",
             "quantize_method",
         )
-        flags_comp_bool = ("fake_vid",)
+        flags_comp_bool = ("fake_vid", "force_pywebp")
         keyword_args: Dict[str, Any]
         for k, v in self.help["comp"].items():
             if k in flags_comp_int:
                 keyword_args = {"type": int, "default": None}
             elif k in flags_comp_float:
                 keyword_args = {"type": float, "default": None}
             elif k in flags_comp_str:
@@ -178,14 +184,15 @@
                     self.compression_presets,  # type: ignore
                     custom_presets,
                 )
             except RuntimeError:
                 print(f"Error: Cannot load custom presets from {args.custom_presets}")
 
         self.cb.no_confirm = args.no_confirm
+        self.cb.no_progress = args.no_progress
 
         self.opt_input = self.get_opt_input(args)
         self.opt_output = self.get_opt_output(args)
         self.opt_comp = self.get_opt_comp(args)
         self.opt_cred = self.get_opt_cred(args)
 
         job = Job(
@@ -379,14 +386,17 @@
             else args.padding_percent,
             steps=self.compression_presets[preset]["steps"]
             if args.steps is None
             else args.steps,
             fake_vid=self.compression_presets[preset]["fake_vid"]
             if args.fake_vid is None
             else args.fake_vid,
+            force_pywebp=self.compression_presets[preset]["force_pywebp"]
+            if args.force_pywebp is None
+            else args.force_pywebp,
             cache_dir=args.cache_dir,
             scale_filter=self.compression_presets[preset]["scale_filter"]
             if args.scale_filter is None
             else args.scale_filter,
             quantize_method=self.compression_presets[preset]["quantize_method"]
             if args.quantize_method is None
             else args.quantize_method,
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/converter.py` & `sticker_convert-2.8.9/src/sticker_convert/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 )
 MSG_REDO_COMP = "[{}] Compressed {} -> {} but size {} {} limit {}, recompressing"
 MSG_DONE_COMP = "[S] Successful compression {} -> {} size {} (step {})"
 MSG_FAIL_COMP = (
     "[F] Failed Compression {} -> {}, "
     "cannot get below limit {} with lowest quality under current settings (Best size: {})"
 )
+MSG_PYWEBP_FLAG_SET = "`--force-pywebp` was set\n"
+MSG_PYWEBP_NO_LIBWEBP = "system WebP>=0.5.0 was not found.\n"
 MSG_PYWEBP_DUPFRAME = (
     "[W] {} contains duplicated frame.\n"
-    "    System WebP>=0.5.0 was not found, hence Pillow cannot be used\n"
-    "    for creating animated webp. Using pywebp instead, which is known to\n"
-    "    collapse same frames into single frame, causing problem with animation timing."
+    "    Using pywebp instead of Pillow as {}"
+    "    This is faster, but known to collapse same frames into single frame,\n"
+    "    causing problem with animation timing."
 )
 MSG_WEBP_PIL_DUPFRAME = (
     "[W] {} contains duplicated frame.\n"
     "    Using Pillow to create animated webp to avoid same frames collapse\n"
     "    into single frame, but this is slower."
 )
 
@@ -714,33 +716,48 @@
             if np.array_equal(frame, prev_frame):
                 return True
             prev_frame = frame
 
         return False
 
     def _frames_export_webp(self) -> None:
+        # TODO: Encode webp with pyav when available
+        # https://github.com/PyAV-Org/PyAV/issues/1352
         has_dup_frames = self._check_dup()
         if self.fps:
             # It was noted that pywebp would collapse all frames.
             # aed005b attempted to fix this by creating webp with
             # variable frame duration. However, the webp created would
             # not be accepted by WhatsApp.
             # Therefore, we are preferring Pillow over pywebp.
             if has_dup_frames:
-                if PIL_WEBP_ANIM:
+                if self.opt_comp.force_pywebp:
+                    if not self.msg_pywebp_dupframe_displayed:
+                        self.cb.put(
+                            MSG_PYWEBP_DUPFRAME.format(
+                                self.in_f_name, MSG_PYWEBP_FLAG_SET
+                            )
+                        )
+                        self.msg_pywebp_dupframe_displayed = True
+                    self._frames_export_pywebp()
+                elif not PIL_WEBP_ANIM:
+                    if not self.msg_pywebp_dupframe_displayed:
+                        self.cb.put(
+                            MSG_PYWEBP_DUPFRAME.format(
+                                self.in_f_name, MSG_PYWEBP_NO_LIBWEBP
+                            )
+                        )
+                        self.msg_pywebp_dupframe_displayed = True
+                    self._frames_export_pywebp()
+                else:
                     # Warn that using Pillow is slower
                     if not self.msg_webp_pil_dupframe_displayed:
                         self.cb.put(MSG_WEBP_PIL_DUPFRAME.format(self.in_f_name))
                         self.msg_webp_pil_dupframe_displayed = True
                     self._frames_export_pil_anim()
-                else:
-                    if not self.msg_pywebp_dupframe_displayed:
-                        self.cb.put(MSG_PYWEBP_DUPFRAME.format(self.in_f_name))
-                        self.msg_pywebp_dupframe_displayed = True
-                    self._frames_export_pywebp()
             else:
                 self._frames_export_pywebp()
         else:
             self._frames_export_pil()
 
     def _frames_export_pil(self) -> None:
         with Image.fromarray(self.frames_processed[0]) as im:  # type: ignore
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/definitions.py` & `sticker_convert-2.8.9/src/sticker_convert/definitions.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_base.py` & `sticker_convert-2.8.9/src/sticker_convert/downloaders/download_base.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_kakao.py` & `sticker_convert-2.8.9/src/sticker_convert/downloaders/download_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_line.py` & `sticker_convert-2.8.9/src/sticker_convert/downloaders/download_line.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_signal.py` & `sticker_convert-2.8.9/src/sticker_convert/downloaders/download_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_telegram.py` & `sticker_convert-2.8.9/src/sticker_convert/downloaders/download_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/downloaders/download_viber.py` & `sticker_convert-2.8.9/src/sticker_convert/downloaders/download_viber.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui.py` & `sticker_convert-2.8.9/src/sticker_convert/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         self.size_disable_var = BooleanVar()
         self.bg_color_var = StringVar()
         self.img_format_var = StringVar(self)
         self.vid_format_var = StringVar(self)
         self.fake_vid_var = BooleanVar()
         self.scale_filter_var = StringVar(self)
         self.quantize_method_var = StringVar(self)
+        self.force_pywebp_var = BooleanVar()
         self.cache_dir_var = StringVar(self)
         self.default_emoji_var = StringVar(self)
         self.steps_var = IntVar(self)
         self.processes_var = IntVar(self)
 
         # Output
         self.output_option_display_var = StringVar(self)
@@ -521,14 +522,15 @@
             else None,
             bg_color=self.bg_color_var.get(),
             padding_percent=self.padding_percent_var.get(),
             steps=self.steps_var.get(),
             fake_vid=self.fake_vid_var.get(),
             scale_filter=self.scale_filter_var.get(),
             quantize_method=self.quantize_method_var.get(),
+            force_pywebp=self.force_pywebp_var.get(),
             cache_dir=self.cache_dir_var.get()
             if self.cache_dir_var.get() != ""
             else None,
             default_emoji=self.default_emoji_var.get(),
             no_compress=self.no_compress_var.get(),
             processes=self.processes_var.get(),
         )
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/comp_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/comp_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         self.gui.vid_size_max_var.set(preset.get("size_max", {}).get("vid"))
         self.gui.img_format_var.set(preset.get("format", {}).get("img"))
         self.gui.vid_format_var.set(preset.get("format", {}).get("vid"))
         self.gui.bg_color_var.set(preset.get("bg_color"))
         self.gui.fake_vid_var.set(preset.get("fake_vid"))
         self.gui.scale_filter_var.set(preset.get("scale_filter"))
         self.gui.quantize_method_var.set(preset.get("quantize_method"))
+        self.gui.force_pywebp_var.set(preset.get("force_pywebp"))
         self.gui.default_emoji_var.set(preset.get("default_emoji"))
         self.gui.steps_var.set(preset.get("steps"))
 
         self.cb_no_compress()
         self.gui.highlight_fields()
 
     def cb_compress_advanced(self, *_: Any) -> None:
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/config_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/config_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/control_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/control_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/cred_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/cred_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/input_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/input_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/output_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/output_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/progress_frame.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/progress_frame.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/frames/right_clicker.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/frames/right_clicker.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/gui_utils.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/gui_utils.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/advanced_compression_window.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/advanced_compression_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,26 @@
             self.gui.quantize_method_var.get(),
             "imagequant",
             "fastoctree",
             "none",
             bootstyle="secondary",  # type: ignore
         )
 
+        self.force_pywebp_help_btn = self.add_help_btn(
+            self.gui.help["comp"]["force_pywebp"]
+        )
+        self.force_pywebp_lbl = Label(self.frame_advcomp, text="Force pywebp")
+        self.force_pywebp_cbox = Checkbutton(
+            self.frame_advcomp,
+            variable=self.gui.force_pywebp_var,
+            onvalue=True,
+            offvalue=False,
+            bootstyle="success-round-toggle",  # type: ignore
+        )
+
         self.cache_dir_help_btn = self.add_help_btn(self.gui.help["comp"]["cache_dir"])
         self.cache_dir_lbl = Label(self.frame_advcomp, text="Custom cache directory")
         self.cache_dir_entry = Entry(
             self.frame_advcomp, textvariable=self.gui.cache_dir_var, width=30
         )
         self.cache_dir_entry.bind("<Button-3><ButtonRelease-3>", RightClicker)
 
@@ -408,14 +420,18 @@
         r += 1
         self.quantize_method_help_btn.grid(column=0, row=r, sticky="w", padx=3, pady=3)
         self.quantize_method_lbl.grid(column=1, row=r, sticky="w", padx=3, pady=3)
         self.quantize_method_opt.grid(
             column=2, row=r, columnspan=4, sticky="nes", padx=3, pady=3
         )
         r += 1
+        self.force_pywebp_help_btn.grid(column=0, row=r, sticky="w", padx=3, pady=3)
+        self.force_pywebp_lbl.grid(column=1, row=r, sticky="w", padx=3, pady=3)
+        self.force_pywebp_cbox.grid(column=6, row=r, sticky="nes", padx=3, pady=3)
+        r += 1
         self.cache_dir_help_btn.grid(column=0, row=r, sticky="w", padx=3, pady=3)
         self.cache_dir_lbl.grid(column=1, row=r, sticky="w", padx=3, pady=3)
         self.cache_dir_entry.grid(
             column=2, row=r, columnspan=4, sticky="nes", padx=3, pady=3
         )
         r += 1
         self.default_emoji_help_btn.grid(column=0, row=r, sticky="w", padx=3, pady=3)
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/base_window.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/base_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/kakao_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/line_get_auth_window.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/line_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/gui_components/windows/signal_get_auth_window.py` & `sticker_convert-2.8.9/src/sticker_convert/gui_components/windows/signal_get_auth_window.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Info.plist`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 1.sticker/Sticker 1.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 2.sticker/Sticker 2.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/Sticker Pack.stickerpack/Sticker 3.sticker/Sticker 3.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/App-Store-1024x1024pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-App-Store-1024x768pt.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-67x50pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPad-Pro-74x55pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages-iPhone-60x45pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages27x20pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/Messages32x24pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPad-Settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-Settings-29pt@3x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers StickerPackExtension/Stickers.xcstickers/iMessage App Icon.stickersiconset/iPhone-settings-29pt@2x.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate` & `sticker_convert-2.8.9/src/sticker_convert/ios-message-stickers-template/stickers.xcodeproj/project.xcworkspace/xcuserdata/niklaspeterson.xcuserdatad/UserInterfaceState.xcuserstate`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/job.py` & `sticker_convert-2.8.9/src/sticker_convert/job.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/job_option.py` & `sticker_convert-2.8.9/src/sticker_convert/job_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     bg_color: Optional[str] = None
 
     padding_percent: int = 0
 
     steps: int = 1
     fake_vid: Optional[bool] = None
     quantize_method: Optional[str] = None
+    force_pywebp: Optional[bool] = None
     scale_filter: Optional[str] = None
     cache_dir: Optional[str] = None
     default_emoji: str = "😀"
     no_compress: Optional[bool] = None
     processes: int = ceil(cpu_count() / 2)
     animated: Optional[bool] = None
     square: Optional[bool] = None
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/NotoColorEmoji.ttf` & `sticker_convert-2.8.9/src/sticker_convert/resources/NotoColorEmoji.ttf`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/appicon.icns` & `sticker_convert-2.8.9/src/sticker_convert/resources/appicon.icns`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/appicon.ico` & `sticker_convert-2.8.9/src/sticker_convert/resources/appicon.ico`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/appicon.png` & `sticker_convert-2.8.9/src/sticker_convert/resources/appicon.png`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/compression.json` & `sticker_convert-2.8.9/src/sticker_convert/resources/compression.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'auto'": "{'force_pywebp': False}",*

 * * "'custom'": "{'force_pywebp': False}",*

 * * "'imessage_large'": "{'force_pywebp': False}",*

 * * "'imessage_medium'": "{'force_pywebp': False}",*

 * * "'imessage_small'": "{'force_pywebp': False}",*

 * * "'kakao'": "{'force_pywebp': False}",*

 * * "'line'": "{'force_pywebp': False}",*

 * * "'signal'": "{'force_pywebp': False}",*

 * * "'telegram'": "{'force_pywebp': False}",*

 * * "'telegram_emoji'": "{'force_pywebp': False}",*

 * * "'viber'": "{'force_pywebp': False}",*

 * * "'whatsapp'": "{'force_pywebp': False}"}*

```diff
@@ -8,14 +8,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 10000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".webm",
             "vid": ".png"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -55,14 +56,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 10000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".webm",
             "vid": ".png"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -102,14 +104,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 2000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".png"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -149,14 +152,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 2000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".png"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -196,14 +200,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 2000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".png"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -243,14 +248,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 5000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".gif"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -290,14 +296,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 4000,
             "min": 83
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".apng"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -337,14 +344,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 3000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".apng"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -384,14 +392,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 3000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".webm"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -431,14 +440,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 3000,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".webm"
         },
         "fps": {
             "max": 30,
             "min": 1,
@@ -478,14 +488,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 0,
             "min": 0
         },
         "fake_vid": false,
+        "force_pywebp": false,
         "format": {
             "img": ".png",
             "vid": ".png"
         },
         "fps": {
             "max": 1,
             "min": 1,
@@ -525,14 +536,15 @@
         },
         "default_emoji": "\ud83d\ude00",
         "duration": {
             "max": 10000,
             "min": 8
         },
         "fake_vid": true,
+        "force_pywebp": false,
         "format": {
             "img": ".webp",
             "vid": ".webp"
         },
         "fps": {
             "max": 30,
             "min": 1,
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/emoji.json` & `sticker_convert-2.8.9/src/sticker_convert/resources/emoji.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/help.json` & `sticker_convert-2.8.9/src/sticker_convert/resources/help.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642276422764227%*

 * *Differences: {"'comp'": "{'force_pywebp': 'Force using pywebp for encoding webp files instead of Pillow.'}",*

 * * "'global'": "{'no_progress': 'Do not show progress bar in CLI.'}"}*

```diff
@@ -7,14 +7,15 @@
         "color_min": "Set minimum number of colors (For converting to apng and apng only).",
         "color_power": "Between -1 and positive infinity. Power lower = More importance of the parameter, try harder to keep higher and not sacrifice.",
         "default_emoji": "Set the default emoji for uploading Signal and Telegram sticker packs.",
         "duration": "Change playback speed if outside of duration limit.\nDuration set in miliseconds.\n0 will disable limit.",
         "duration_max": "Set maximum output duration in miliseconds.",
         "duration_min": "Set minimum output duration in miliseconds.",
         "fake_vid": "Convert (faking) image to video.\nUseful if:\n(1) Size limit for video is larger than image;\n(2) Mix image and video into same pack.",
+        "force_pywebp": "Force using pywebp for encoding webp files instead of Pillow.",
         "format": "Set file format for video and image.",
         "fps": "FPS Higher = Smoother but larger size.",
         "fps_max": "Set maximum output fps.",
         "fps_min": "Set minimum output fps.",
         "fps_power": "Between -1 and positive infinity. Power lower = More importance of the parameter, try harder to keep higher and not sacrifice.",
         "img_format": "Set file format if input is static.",
         "img_size_max": "Set maximum file size limit for static stickers.",
@@ -56,15 +57,16 @@
         "signal_password": "Set Signal password. Required for uploading Signal stickers.",
         "signal_uuid": "Set Signal uuid. Required for uploading Signal stickers.",
         "telegram_token": "Set Telegram token. Required for uploading and downloading Telegram stickers.",
         "telegram_userid": "Set telegram user_id (From real account, not bot account). Required for uploading Telegram stickers."
     },
     "global": {
         "custom_presets": "Specify a json file containing custom compression presets.\nSee compression.json for format.\nNote that if present, 'custom_preset.json' from config directory would be auto loaded.",
-        "no_confirm": "Do not ask any questions."
+        "no_confirm": "Do not ask any questions.",
+        "no_progress": "Do not show progress bar in CLI."
     },
     "input": {
         "input_dir": "Specify input directory."
     },
     "output": {
         "author": "Set author of created sticker pack.",
         "output_dir": "Specify output directory.",
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/input.json` & `sticker_convert-2.8.9/src/sticker_convert/resources/input.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/resources/output.json` & `sticker_convert-2.8.9/src/sticker_convert/resources/output.json`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/uploaders/compress_wastickers.py` & `sticker_convert-2.8.9/src/sticker_convert/uploaders/compress_wastickers.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_base.py` & `sticker_convert-2.8.9/src/sticker_convert/uploaders/upload_base.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_signal.py` & `sticker_convert-2.8.9/src/sticker_convert/uploaders/upload_signal.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/uploaders/upload_telegram.py` & `sticker_convert-2.8.9/src/sticker_convert/uploaders/upload_telegram.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/uploaders/xcode_imessage.py` & `sticker_convert-2.8.9/src/sticker_convert/uploaders/xcode_imessage.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_kakao_auth.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/auth/get_kakao_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_line_auth.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/auth/get_line_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/auth/get_signal_auth.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/auth/get_signal_auth.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/callback.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         msg: Optional[Callable[..., None]] = None,
         bar: Optional[Callable[..., None]] = None,
         msg_block: Optional[Callable[..., None]] = None,
         ask_bool: Optional[Callable[..., bool]] = None,
         ask_str: Optional[Callable[..., str]] = None,
         silent: bool = False,
         no_confirm: bool = False,
+        no_progress: bool = False,
     ) -> None:
         self.progress_bar: Optional[tqdm[Any]] = None
 
         if msg:
             self.msg = msg
         else:
             self.msg = self.cb_msg
@@ -87,14 +88,15 @@
         if ask_str:
             self.ask_str = ask_str
         else:
             self.ask_str = self.cb_ask_str
 
         self.silent = silent
         self.no_confirm = no_confirm
+        self.no_progress = no_progress
 
     def cb_msg(self, *args: Any, **kwargs: Any) -> None:
         if self.silent:
             return
 
         msg = kwargs.get("msg")
 
@@ -109,15 +111,15 @@
 
     def cb_bar(
         self,
         set_progress_mode: Optional[str] = None,
         steps: int = 0,
         update_bar: int = 0,
     ) -> None:
-        if self.silent:
+        if self.silent or self.no_progress:
             return
 
         if self.progress_bar:
             if update_bar:
                 self.progress_bar.update(update_bar)
             elif set_progress_mode in ("indeterminate", "clear"):
                 self.progress_bar.close()
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/files/cache_store.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/files/cache_store.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/files/json_manager.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/files/json_manager.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/files/json_resources_loader.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/files/json_resources_loader.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/files/metadata_handler.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/files/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/files/run_bin.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/files/run_bin.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/files/sanitize_filename.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/files/sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/media/apple_png_normalize.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/media/apple_png_normalize.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/media/codec_info.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/media/codec_info.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/media/decrypt_kakao.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/media/decrypt_kakao.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/media/format_verify.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/media/format_verify.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert/utils/url_detect.py` & `sticker_convert-2.8.9/src/sticker_convert/utils/url_detect.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/src/sticker_convert.egg-info/PKG-INFO` & `sticker_convert-2.8.9/src/sticker_convert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sticker-convert
-Version: 2.8.8
+Version: 2.8.9
 Summary: Convert (animated) stickers to/from WhatsApp, Telegram, Signal, Line, Kakao, Viber, iMessage. Written in Python.
 Author-email: laggykiller <chaudominic2@gmail.com>
 Maintainer-email: laggykiller <chaudominic2@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
@@ -475,44 +475,49 @@
 7. Enter credentials if you want to download/upload from telegram or upload from Signal (View 'Compatability' and 'FAQ' section for more information)
 8. Press 'Start'
 
 ## How to use (CLI)
 To run in CLI mode, pass on any arguments
 
 ```
-usage: sticker-convert.py [-h] [--version] [--no-confirm] [--custom-presets CUSTOM_PRESETS] [--input-dir INPUT_DIR]
+usage: sticker-convert.py [-h] [--version] [--no-confirm] [--no-progress] [--custom-presets CUSTOM_PRESETS] [--input-dir INPUT_DIR]
                           [--download-auto DOWNLOAD_AUTO | --download-signal DOWNLOAD_SIGNAL | --download-telegram DOWNLOAD_TELEGRAM | --download-line DOWNLOAD_LINE | --download-kakao DOWNLOAD_KAKAO | --download-viber DOWNLOAD_VIBER]
-                          [--output-dir OUTPUT_DIR] [--author AUTHOR] [--title TITLE] [--export-signal | --export-telegram | --export-telegram-emoji | --export-whatsapp | --export-imessage]
-                          [--no-compress] [--preset {auto,signal,telegram,telegram_emoji,whatsapp,line,kakao,viber,imessage_small,imessage_medium,imessage_large,custom}] [--steps STEPS]
-                          [--processes PROCESSES] [--fps-min FPS_MIN] [--fps-max FPS_MAX] [--fps-power FPS_POWER] [--res-min RES_MIN] [--res-max RES_MAX] [--res-w-min RES_W_MIN] [--res-w-max RES_W_MAX]
-                          [--res-h-min RES_H_MIN] [--res-h-max RES_H_MAX] [--res-power RES_POWER] [--quality-min QUALITY_MIN] [--quality-max QUALITY_MAX] [--quality-power QUALITY_POWER]
-                          [--color-min COLOR_MIN] [--color-max COLOR_MAX] [--color-power COLOR_POWER] [--duration-min DURATION_MIN] [--duration-max DURATION_MAX] [--padding-percent PADDING_PERCENT]
-                          [--bg-color BG_COLOR] [--vid-size-max VID_SIZE_MAX] [--img-size-max IMG_SIZE_MAX] [--vid-format VID_FORMAT] [--img-format IMG_FORMAT] [--fake-vid] [--scale-filter SCALE_FILTER]
-                          [--quantize-method QUANTIZE_METHOD] [--cache-dir CACHE_DIR] [--default-emoji DEFAULT_EMOJI] [--signal-uuid SIGNAL_UUID] [--signal-password SIGNAL_PASSWORD] [--signal-get-auth]
-                          [--signal-data-dir SIGNAL_DATA_DIR] [--telegram-token TELEGRAM_TOKEN] [--telegram-userid TELEGRAM_USERID] [--kakao-auth-token KAKAO_AUTH_TOKEN] [--kakao-get-auth]
-                          [--kakao-username KAKAO_USERNAME] [--kakao-password KAKAO_PASSWORD] [--kakao-country-code KAKAO_COUNTRY_CODE] [--kakao-phone-number KAKAO_PHONE_NUMBER] [--line-get-auth]
-                          [--line-cookies LINE_COOKIES] [--save-cred SAVE_CRED]
+                          [--output-dir OUTPUT_DIR] [--author AUTHOR] [--title TITLE]
+                          [--export-signal | --export-telegram | --export-telegram-emoji | --export-whatsapp | --export-imessage] [--no-compress]
+                          [--preset {auto,signal,telegram,telegram_emoji,whatsapp,line,kakao,viber,imessage_small,imessage_medium,imessage_large,custom}]
+                          [--steps STEPS] [--processes PROCESSES] [--fps-min FPS_MIN] [--fps-max FPS_MAX] [--fps-power FPS_POWER] [--res-min RES_MIN]
+                          [--res-max RES_MAX] [--res-w-min RES_W_MIN] [--res-w-max RES_W_MAX] [--res-h-min RES_H_MIN] [--res-h-max RES_H_MAX]
+                          [--res-power RES_POWER] [--quality-min QUALITY_MIN] [--quality-max QUALITY_MAX] [--quality-power QUALITY_POWER] [--color-min COLOR_MIN]
+                          [--color-max COLOR_MAX] [--color-power COLOR_POWER] [--duration-min DURATION_MIN] [--duration-max DURATION_MAX]
+                          [--padding-percent PADDING_PERCENT] [--bg-color BG_COLOR] [--vid-size-max VID_SIZE_MAX] [--img-size-max IMG_SIZE_MAX]
+                          [--vid-format VID_FORMAT] [--img-format IMG_FORMAT] [--fake-vid] [--scale-filter SCALE_FILTER] [--quantize-method QUANTIZE_METHOD]
+                          [--force-pywebp] [--cache-dir CACHE_DIR] [--default-emoji DEFAULT_EMOJI] [--signal-uuid SIGNAL_UUID] [--signal-password SIGNAL_PASSWORD]
+                          [--signal-get-auth] [--signal-data-dir SIGNAL_DATA_DIR] [--telegram-token TELEGRAM_TOKEN] [--telegram-userid TELEGRAM_USERID]
+                          [--kakao-auth-token KAKAO_AUTH_TOKEN] [--kakao-get-auth] [--kakao-username KAKAO_USERNAME] [--kakao-password KAKAO_PASSWORD]
+                          [--kakao-country-code KAKAO_COUNTRY_CODE] [--kakao-phone-number KAKAO_PHONE_NUMBER] [--line-get-auth] [--line-cookies LINE_COOKIES]
+                          [--save-cred SAVE_CRED]
 
 CLI for stickers-convert
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   --no-confirm          Do not ask any questions.
+  --no-progress         Do not show progress bar in CLI.
   --custom-presets CUSTOM_PRESETS
                         Specify a json file containing custom compression presets.
                         See compression.json for format.
                         Note that if present, 'custom_preset.json' from config directory would be auto loaded.
 
 Input options:
   --input-dir INPUT_DIR
                         Specify input directory.
   --download-auto DOWNLOAD_AUTO
                         Auto detect URL type and download
-                        (Supported input sources: Signal, Telegram, Line, Kakao)
+                        (Supported input sources: Signal, Telegram, Line, Kakao, Viber)
   --download-signal DOWNLOAD_SIGNAL
                         Download signal stickers from a URL as input
                         (Example: https://signal.art/addstickers/#pack_id=xxxxx&pack_key=xxxxx)
   --download-telegram DOWNLOAD_TELEGRAM
                         Download telegram stickers from a URL as input
                         (Example: https://telegram.me/addstickers/xxxxx
                          OR https://telegram.me/addemoji/xxxxx)
@@ -583,15 +588,15 @@
   --duration-min DURATION_MIN
                         Set minimum output duration in miliseconds.
   --duration-max DURATION_MAX
                         Set maximum output duration in miliseconds.
   --padding-percent PADDING_PERCENT
                         Set percentage of space used as padding.
   --bg-color BG_COLOR   Set custom background color in rrggbbaa format.
-                        Example: 00ff00 for green with alpha 0.
+                        Example: 00ff0000 for green with alpha 0.
                         If this is not set, background color would be auto set to black if image is bright, or white if image is dark.
                         Note: The color should not be visible if output format supports transparency.
   --vid-size-max VID_SIZE_MAX
                         Set maximum file size limit for animated stickers.
   --img-size-max IMG_SIZE_MAX
                         Set maximum file size limit for static stickers.
   --vid-format VID_FORMAT
@@ -611,14 +616,15 @@
                         - bicubic = Cubic spline interpolation
                         - lanczos = A high-quality downsampling filter
   --quantize-method QUANTIZE_METHOD
                         Set method for quantizing image. Default as imagequant. Valid options are:
                         - imagequant = Best quality but slow
                         - fastoctree = Fast but image looks chunky
                         - none = No image quantizing, large image size as result
+  --force-pywebp        Force using pywebp for encoding webp files instead of Pillow.
   --cache-dir CACHE_DIR
                         Set custom cache directory.
                         Useful for debugging, or speed up conversion if cache_dir is on RAM disk.
   --default-emoji DEFAULT_EMOJI
                         Set the default emoji for uploading Signal and Telegram sticker packs.
 
 Credentials options:
```

### Comparing `sticker_convert-2.8.8/src/sticker_convert.egg-info/SOURCES.txt` & `sticker_convert-2.8.9/src/sticker_convert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/tests/test_compression.py` & `sticker_convert-2.8.9/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/tests/test_download.py` & `sticker_convert-2.8.9/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `sticker_convert-2.8.8/tests/test_export.py` & `sticker_convert-2.8.9/tests/test_export.py`

 * *Files identical despite different names*

