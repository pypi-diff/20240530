# Comparing `tmp/vht-0.3.69.tar.gz` & `tmp/vht-0.3.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vht-0.3.69.tar", last modified: Sun Apr 28 23:48:37 2024, max compression
+gzip compressed data, was "vht-0.3.96.tar", last modified: Wed May 29 22:34:47 2024, max compression
```

## Comparing `vht-0.3.69.tar` & `vht-0.3.96.tar`

### file list

```diff
@@ -1,138 +1,140 @@
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.426646 vht-0.3.69/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2022-12-31 13:17:54.000000 vht-0.3.69/LICENSE
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       49 2022-12-31 13:17:54.000000 vht-0.3.69/MANIFEST.in
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1912 2024-04-28 23:48:37.426646 vht-0.3.69/PKG-INFO
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1194 2023-08-11 00:51:13.000000 vht-0.3.69/README.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/data/
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/data/bank/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2022-12-31 13:17:54.000000 vht-0.3.69/data/bank/10-gm1
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2022-12-31 13:17:54.000000 vht-0.3.69/data/bank/20-gm2
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      290 2022-12-31 13:17:54.000000 vht-0.3.69/data/com.github.rdybka.vht.desktop
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/data/ctrl/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      294 2022-12-31 13:17:54.000000 vht-0.3.69/data/ctrl/10-gm
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      166 2022-12-31 13:17:54.000000 vht-0.3.69/data/ctrl/20-zyn
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2022-12-31 13:17:54.000000 vht-0.3.69/data/mandy.png
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2022-12-31 13:17:54.000000 vht-0.3.69/data/menu.ui
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2022-12-31 13:17:54.000000 vht-0.3.69/data/vht.png
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2022-12-31 13:17:54.000000 vht-0.3.69/data/vht.svg
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.402646 vht-0.3.69/doc/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2364 2024-04-28 23:29:39.000000 vht-0.3.69/doc/vht.1.gz
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4643 2024-04-28 23:29:30.000000 vht-0.3.69/doc/vht.1.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.414646 vht-0.3.69/libvht/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       75 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/__init__.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/ctrlrow.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/ctrlrow.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7095 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/envelope.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/envelope.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1961 2024-04-20 19:24:40.000000 vht-0.3.69/libvht/jack_process.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/jack_process.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-04-28 12:26:17.000000 vht-0.3.69/libvht/libcvht.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-04-28 23:29:38.000000 vht-0.3.69/libvht/libcvht.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-04-28 23:29:38.000000 vht-0.3.69/libvht/libcvht_wrap.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8287 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/libvht.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    34608 2024-04-08 16:06:43.000000 vht-0.3.69/libvht/mandy.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2023-03-31 14:55:44.000000 vht-0.3.69/libvht/mandy.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/mandy_pix_scan.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/mandy_pix_scan.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/mandy_trk_disp.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      986 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/mandy_trk_disp.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17029 2024-04-20 19:24:40.000000 vht-0.3.69/libvht/midi_client.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4512 2024-04-14 23:40:36.000000 vht-0.3.69/libvht/midi_client.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/midi_event.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/midi_event.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    16010 2024-04-22 08:56:08.000000 vht-0.3.69/libvht/module.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-04-22 08:54:58.000000 vht-0.3.69/libvht/module.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3036 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/row.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/row.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28979 2024-04-28 13:47:56.000000 vht-0.3.69/libvht/sequence.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4502 2024-04-28 12:25:10.000000 vht-0.3.69/libvht/sequence.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6457 2024-04-22 10:40:58.000000 vht-0.3.69/libvht/smf.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-04-22 08:52:28.000000 vht-0.3.69/libvht/smf.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-04-20 23:47:04.000000 vht-0.3.69/libvht/stolen.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    29202 2023-03-23 02:07:54.000000 vht-0.3.69/libvht/timeline.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2022-12-31 13:17:54.000000 vht-0.3.69/libvht/timeline.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    41059 2023-03-21 08:03:40.000000 vht-0.3.69/libvht/track.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2023-01-30 08:43:51.000000 vht-0.3.69/libvht/track.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-04-08 11:52:27.000000 vht-0.3.69/libvht/tracy.c
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-04-08 11:52:18.000000 vht-0.3.69/libvht/tracy.h
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtcolumn.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtctrl.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtctrllist.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtctrlrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtextras.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtmandy.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-04-22 09:54:53.000000 vht-0.3.69/libvht/vhtmodule.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-04-14 19:43:50.000000 vht-0.3.69/libvht/vhtport.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-04-09 00:56:37.000000 vht-0.3.69/libvht/vhtports.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtquicklist.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhtrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-04-28 12:27:13.000000 vht-0.3.69/libvht/vhtsequence.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimeline.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinechange.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinechanges.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelineloop.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelineslices.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinestrip.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelinestrips.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttimelineticks.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttrack.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2023-03-21 08:03:58.000000 vht-0.3.69/libvht/vhttracy.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1791 2024-04-28 23:44:34.000000 vht-0.3.69/pyproject.toml
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-04-28 23:48:37.426646 vht-0.3.69/setup.cfg
--rwxr--r--   0 mal1ce    (1000) mal1ce    (1000)     1837 2024-04-28 23:32:00.000000 vht-0.3.69/setup.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.422646 vht-0.3.69/vht/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)      124 2022-12-31 13:17:54.000000 vht-0.3.69/vht/__init__.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2023-03-21 08:04:15.000000 vht-0.3.69/vht/autoexec.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2023-03-21 08:04:15.000000 vht-0.3.69/vht/bankcfg.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-04-26 02:28:28.000000 vht-0.3.69/vht/capturebutton.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-04-28 13:24:55.000000 vht-0.3.69/vht/codedaemon.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-04-22 09:13:03.000000 vht-0.3.69/vht/configuration.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2023-03-21 08:04:15.000000 vht-0.3.69/vht/console.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllereditor.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllersview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     5705 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllersviewrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2023-03-21 08:04:15.000000 vht-0.3.69/vht/controllerundobuffer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2023-03-21 08:04:15.000000 vht-0.3.69/vht/ctrlcfg.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2023-03-21 08:04:15.000000 vht-0.3.69/vht/extras.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2023-03-21 08:04:15.000000 vht-0.3.69/vht/filerotator.py
--rwxr--r--   0 mal1ce    (1000) mal1ce    (1000)    11500 2024-04-27 16:39:10.000000 vht-0.3.69/vht/main.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    18460 2024-04-28 12:22:47.000000 vht-0.3.69/vht/mainwin.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2023-03-21 08:04:15.000000 vht-0.3.69/vht/mandymenu.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-04-08 12:16:06.000000 vht-0.3.69/vht/mandyview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2023-03-21 08:04:15.000000 vht-0.3.69/vht/midimapview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2023-03-21 08:04:15.000000 vht-0.3.69/vht/midimapviewrow.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2023-03-21 08:04:15.000000 vht-0.3.69/vht/notebooklabel.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-03-22 16:50:28.000000 vht-0.3.69/vht/poormanspiano.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-04-14 21:33:38.000000 vht-0.3.69/vht/portconfig.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2023-03-21 08:04:15.000000 vht-0.3.69/vht/portconfigpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     7615 2024-04-14 19:32:45.000000 vht-0.3.69/vht/portconfigview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    24666 2024-04-22 09:57:34.000000 vht-0.3.69/vht/preferenceswin.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2023-03-21 08:04:15.000000 vht-0.3.69/vht/probeditor.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2023-03-21 08:04:15.000000 vht-0.3.69/vht/propview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2023-03-21 08:04:15.000000 vht-0.3.69/vht/pulsar.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2023-03-21 08:04:15.000000 vht-0.3.69/vht/randomcomposer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8290 2024-04-22 09:54:53.000000 vht-0.3.69/vht/renderer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9639 2024-04-21 16:33:45.000000 vht-0.3.69/vht/renderwin.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2023-03-21 08:04:15.000000 vht-0.3.69/vht/sequencelistview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    13092 2024-04-28 12:53:09.000000 vht-0.3.69/vht/sequencelistviewpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2023-03-21 08:04:15.000000 vht-0.3.69/vht/sequencepropviewpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2023-03-21 12:19:50.000000 vht-0.3.69/vht/sequencetriggersview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-04-28 00:39:42.000000 vht-0.3.69/vht/sequenceview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6678 2023-03-21 08:04:15.000000 vht-0.3.69/vht/shortcutmayhem.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-03-22 16:23:30.000000 vht-0.3.69/vht/sidetrackview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    19524 2023-09-09 20:22:06.000000 vht-0.3.69/vht/statusbar.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2023-03-21 08:04:15.000000 vht-0.3.69/vht/thumbmanager.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2023-03-21 08:04:15.000000 vht-0.3.69/vht/timelineview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2023-03-21 08:04:15.000000 vht-0.3.69/vht/timeshifteditor.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2023-03-21 08:04:15.000000 vht-0.3.69/vht/trackpropview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-04-08 23:20:41.000000 vht-0.3.69/vht/trackpropviewpopover.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2023-03-21 08:04:15.000000 vht-0.3.69/vht/trackundobuffer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)    96092 2024-03-22 15:55:48.000000 vht-0.3.69/vht/trackview.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2023-03-21 08:04:15.000000 vht-0.3.69/vht/trackviewpointer.py
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2023-03-21 08:04:15.000000 vht-0.3.69/vht/velocityeditor.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-04-28 23:48:37.426646 vht-0.3.69/vht.egg-info/
--rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1912 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2518 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/SOURCES.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/dependency_links.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       37 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/entry_points.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-04-28 23:48:37.000000 vht-0.3.69/vht.egg-info/top_level.txt
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.417472 vht-0.3.96/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2024-05-08 12:01:32.000000 vht-0.3.96/LICENSE
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2024-05-08 12:01:32.000000 vht-0.3.96/MANIFEST.in
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1874 2024-05-29 22:34:47.417472 vht-0.3.96/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1147 2024-05-28 20:35:49.000000 vht-0.3.96/README.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.401471 vht-0.3.96/data/
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.401471 vht-0.3.96/data/bank/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2024-05-08 12:01:32.000000 vht-0.3.96/data/bank/10-gm1
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2024-05-08 12:01:32.000000 vht-0.3.96/data/bank/20-gm2
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.401471 vht-0.3.96/data/ctrl/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2024-05-08 12:01:32.000000 vht-0.3.96/data/ctrl/10-gm
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2024-05-08 12:01:32.000000 vht-0.3.96/data/ctrl/20-zyn
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2024-05-08 12:01:32.000000 vht-0.3.96/data/mandy.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2024-05-08 12:01:32.000000 vht-0.3.96/data/menu.ui
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      318 2024-05-29 20:04:45.000000 vht-0.3.96/data/net.sourceforge.projects.vht.desktop
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2095 2024-05-29 22:05:35.000000 vht-0.3.96/data/net.sourceforge.projects.vht.metainfo.xml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-29 19:42:46.000000 vht-0.3.96/data/net.sourceforge.projects.vht.svg
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2024-05-08 12:01:32.000000 vht-0.3.96/data/vht.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-08 12:01:32.000000 vht-0.3.96/data/vht.svg
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.401471 vht-0.3.96/doc/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2362 2024-05-28 20:42:27.000000 vht-0.3.96/doc/vht.1.gz
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4641 2024-05-28 20:22:40.000000 vht-0.3.96/doc/vht.1.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.409471 vht-0.3.96/libvht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/ctrlrow.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/ctrlrow.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7088 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/envelope.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/envelope.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2121 2024-05-29 20:50:11.000000 vht-0.3.96/libvht/jack_process.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/jack_process.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/libcvht.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-05-29 22:18:46.000000 vht-0.3.96/libvht/libcvht.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-05-29 22:18:46.000000 vht-0.3.96/libvht/libcvht_wrap.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7542 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/libvht.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34594 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/mandy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/mandy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/mandy_pix_scan.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/mandy_pix_scan.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/mandy_trk_disp.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/mandy_trk_disp.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17045 2024-05-27 12:13:59.000000 vht-0.3.96/libvht/midi_client.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4531 2024-05-27 12:12:54.000000 vht-0.3.96/libvht/midi_client.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/midi_event.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/midi_event.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15996 2024-05-27 12:02:48.000000 vht-0.3.96/libvht/module.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/module.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3029 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/row.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/row.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28972 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/sequence.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4503 2024-05-15 11:24:39.000000 vht-0.3.96/libvht/sequence.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6493 2024-05-08 12:02:30.000000 vht-0.3.96/libvht/smf.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/smf.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/stolen.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29373 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/timeline.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/timeline.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41038 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/track.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/track.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/tracy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/tracy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtcolumn.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtctrl.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtctrllist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtctrlrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtextras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtmandy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtmodule.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtport.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtports.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtquicklist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2024-05-27 12:45:52.000000 vht-0.3.96/libvht/vhtrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhtsequence.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimeline.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelinechange.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelinechanges.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelineloop.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelineslices.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelinestrip.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelinestrips.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttimelineticks.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2024-05-27 13:05:52.000000 vht-0.3.96/libvht/vhttrack.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2024-05-08 12:01:32.000000 vht-0.3.96/libvht/vhttracy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1918 2024-05-29 22:18:03.000000 vht-0.3.96/pyproject.toml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-05-29 22:34:47.417472 vht-0.3.96/setup.cfg
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1975 2024-05-29 22:17:44.000000 vht-0.3.96/setup.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.417472 vht-0.3.96/vht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2024-05-08 12:01:32.000000 vht-0.3.96/vht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2024-05-08 12:01:32.000000 vht-0.3.96/vht/autoexec.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2024-05-08 12:01:32.000000 vht-0.3.96/vht/bankcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-05-08 12:01:32.000000 vht-0.3.96/vht/capturebutton.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-05-08 12:01:32.000000 vht-0.3.96/vht/codedaemon.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-05-08 12:01:32.000000 vht-0.3.96/vht/configuration.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2024-05-08 12:01:32.000000 vht-0.3.96/vht/console.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2024-05-09 10:48:54.000000 vht-0.3.96/vht/controllereditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2024-05-08 12:01:32.000000 vht-0.3.96/vht/controllersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5707 2024-05-08 12:01:32.000000 vht-0.3.96/vht/controllersviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2024-05-08 12:01:32.000000 vht-0.3.96/vht/controllerundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2024-05-08 12:01:32.000000 vht-0.3.96/vht/ctrlcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2024-05-08 12:01:32.000000 vht-0.3.96/vht/extras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2024-05-08 12:01:32.000000 vht-0.3.96/vht/filerotator.py
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11519 2024-05-28 22:30:25.000000 vht-0.3.96/vht/main.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18670 2024-05-29 18:58:50.000000 vht-0.3.96/vht/mainwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2024-05-08 12:01:32.000000 vht-0.3.96/vht/mandymenu.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-05-08 12:01:32.000000 vht-0.3.96/vht/mandyview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2024-05-08 12:01:32.000000 vht-0.3.96/vht/midimapview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2024-05-08 12:01:32.000000 vht-0.3.96/vht/midimapviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2024-05-08 12:01:32.000000 vht-0.3.96/vht/notebooklabel.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-05-08 12:01:32.000000 vht-0.3.96/vht/poormanspiano.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-05-08 12:01:32.000000 vht-0.3.96/vht/portconfig.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2024-05-08 12:01:32.000000 vht-0.3.96/vht/portconfigpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7770 2024-05-28 19:34:11.000000 vht-0.3.96/vht/portconfigview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24678 2024-05-28 18:53:13.000000 vht-0.3.96/vht/preferenceswin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2024-05-08 12:01:32.000000 vht-0.3.96/vht/probeditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2024-05-08 12:01:32.000000 vht-0.3.96/vht/propview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2024-05-08 12:01:32.000000 vht-0.3.96/vht/pulsar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2024-05-08 12:01:32.000000 vht-0.3.96/vht/randomcomposer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8188 2024-05-28 20:16:35.000000 vht-0.3.96/vht/renderer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9640 2024-05-27 12:29:20.000000 vht-0.3.96/vht/renderwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2024-05-08 12:01:32.000000 vht-0.3.96/vht/sequencelistview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    13404 2024-05-29 20:09:20.000000 vht-0.3.96/vht/sequencelistviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2024-05-08 12:01:32.000000 vht-0.3.96/vht/sequencepropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2024-05-08 12:01:32.000000 vht-0.3.96/vht/sequencetriggersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-05-08 12:01:32.000000 vht-0.3.96/vht/sequenceview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6644 2024-05-29 18:59:49.000000 vht-0.3.96/vht/shortcutmayhem.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-05-08 12:01:32.000000 vht-0.3.96/vht/sidetrackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2024-05-08 12:01:32.000000 vht-0.3.96/vht/statusbar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2024-05-08 12:01:32.000000 vht-0.3.96/vht/thumbmanager.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2024-05-08 12:01:32.000000 vht-0.3.96/vht/timelineview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2024-05-08 12:01:32.000000 vht-0.3.96/vht/timeshifteditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2024-05-08 12:01:32.000000 vht-0.3.96/vht/trackpropview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-05-08 12:01:32.000000 vht-0.3.96/vht/trackpropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2024-05-08 12:01:32.000000 vht-0.3.96/vht/trackundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    96428 2024-05-15 11:23:14.000000 vht-0.3.96/vht/trackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2024-05-08 12:01:32.000000 vht-0.3.96/vht/trackviewpointer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2024-05-08 12:01:32.000000 vht-0.3.96/vht/velocityeditor.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-29 22:34:47.417472 vht-0.3.96/vht.egg-info/
+-rw-r--r--   0 mal1ce    (1000) mal1ce    (1000)     1874 2024-05-29 22:34:47.000000 vht-0.3.96/vht.egg-info/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2610 2024-05-29 22:34:47.000000 vht-0.3.96/vht.egg-info/SOURCES.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-05-29 22:34:47.000000 vht-0.3.96/vht.egg-info/dependency_links.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       37 2024-05-29 22:34:47.000000 vht-0.3.96/vht.egg-info/entry_points.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-05-29 22:34:47.000000 vht-0.3.96/vht.egg-info/top_level.txt
```

### Comparing `vht-0.3.69/LICENSE` & `vht-0.3.96/LICENSE`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/PKG-INFO` & `vht-0.3.96/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.69
-Summary: vahatraker - a live MIDI sequencer for JACK
+Version: 0.3.96
+Summary: vahatraker - a live MIDI sequencer for pipewire/JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Intended Audience :: End Users/Desktop
@@ -28,15 +28,15 @@
 - live editing
 - fast workflow
 - intuitive midi-in
 - unheard of time signatures
 - scenes a'la 'ton
 - fractal turtles
 - fits on a floppy
-- doesn't make sound
+- doesn't make a sound
 
 Frankly speaking, vht was envisaged as a re-creation
 of seq24 in tracker form for author's "studio needs"
 and offers similar functionality (and limitations).
 It relies 100% on JACK audio connection kit for 
 input/output/synch and uses jack_capture for rendering.
 The GUI has similar dependencies as gnome-calculator
@@ -46,15 +46,13 @@
 Low level stuff was done in C and wrapped in Python.
 Human interfacing part of contraption employs
 GTK through gobject introspection and was also contrived
 in the language we shall no longer spam about.
 
 ## dependencies
 ```
-fedora - jack-audio-connection-kit-devel jack_capture
-ubuntu - libjack-jackd2-dev jack-capture
+pipewire-audio-client-libraries [jack_capture]
 ```
-
 ## install
 ```
 pip3 install vht
 ```
```

### Comparing `vht-0.3.69/README.md` & `vht-0.3.96/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - live editing
 - fast workflow
 - intuitive midi-in
 - unheard of time signatures
 - scenes a'la 'ton
 - fractal turtles
 - fits on a floppy
-- doesn't make sound
+- doesn't make a sound
 
 Frankly speaking, vht was envisaged as a re-creation
 of seq24 in tracker form for author's "studio needs"
 and offers similar functionality (and limitations).
 It relies 100% on JACK audio connection kit for 
 input/output/synch and uses jack_capture for rendering.
 The GUI has similar dependencies as gnome-calculator
@@ -27,15 +27,13 @@
 Low level stuff was done in C and wrapped in Python.
 Human interfacing part of contraption employs
 GTK through gobject introspection and was also contrived
 in the language we shall no longer spam about.
 
 ## dependencies
 ```
-fedora - jack-audio-connection-kit-devel jack_capture
-ubuntu - libjack-jackd2-dev jack-capture
+pipewire-audio-client-libraries [jack_capture]
 ```
-
 ## install
 ```
 pip3 install vht
 ```
```

### Comparing `vht-0.3.69/data/bank/10-gm1` & `vht-0.3.96/data/bank/10-gm1`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/data/bank/20-gm2` & `vht-0.3.96/data/bank/20-gm2`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/data/mandy.png` & `vht-0.3.96/data/mandy.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/data/menu.ui` & `vht-0.3.96/data/menu.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/data/vht.png` & `vht-0.3.96/data/vht.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/data/vht.svg` & `vht-0.3.96/data/net.sourceforge.projects.vht.svg`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/doc/vht.1.md` & `vht-0.3.96/doc/vht.1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% VHT(1) vht 0.3.69
+% VHT(1) vht 0.3.96
 % Remigiusz Dybka
-% April 2024
+% May 2024
 
 # NAME
 **vht** - a minimalistic MIDI sequencer for JACK/GNOME
 
 # SYNOPSIS
 **vht** [file]
```

### Comparing `vht-0.3.69/libvht/ctrlrow.c` & `vht-0.3.96/libvht/ctrlrow.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/ctrlrow.h` & `vht-0.3.96/libvht/ctrlrow.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/envelope.c` & `vht-0.3.96/libvht/envelope.c`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 	return (int)((float)((env_node *)a)->y - (float)((env_node *)b)->y);
 }
 
 void envelope_sort_nodes(envelope *env) {
 	qsort(env->nodes, env->nnodes, sizeof(env_node), env_node_compare);
 }
 
-inline int y2bz(envelope *env, float y) {
+int y2bz(envelope *env, float y) {
 	return (int)y * env->res + (int)((y - floorf(y)) * env->res);
 }
 
 // with regards to my C mentor - Konrad Wicyński
 void envelope_draw_cluster(envelope *env, int nf, int nl) {
 	float lx = 0;					// past
 	float ly = 0;
```

### Comparing `vht-0.3.69/libvht/envelope.h` & `vht-0.3.96/libvht/envelope.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/jack_process.c` & `vht-0.3.96/libvht/jack_process.c`

 * *Files 11% similar despite different names*

```diff
@@ -29,16 +29,26 @@
 
 	midi_client *clt = (midi_client *)arg;
 	module *mod = (module *)clt->mod_ref;
 
 	jack_get_cycle_times(clt->jack_client, &curr_frames, &curr_usecs, &next_usecs, &period_usecs);
 	midi_synch_output_ports(clt);
 
+	if (curr_frames < clt->jack_last_frame) { // drop-out
+		curr_frames = clt->jack_last_frame + nframes;
+	}
+
+	if (clt->freewheeling) {
+		curr_frames = clt->jack_last_frame + nframes;
+	}
+
 	module_advance(mod, curr_frames);
-	clt->jack_last_frame = jack_last_frame_time(clt->jack_client);
+
+	clt->jack_last_frame = curr_frames;
+
 	midi_buffer_flush(clt);
 
 	return 0;
 }
 
 int jack_sample_rate_changed(jack_nframes_t srate, void *arg) {
 	((midi_client *)arg)->jack_sample_rate = srate;
```

### Comparing `vht-0.3.69/libvht/jack_process.h` & `vht-0.3.96/libvht/jack_process.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/libcvht.h` & `vht-0.3.96/libvht/libcvht.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/libcvht.py` & `vht-0.3.96/libvht/libcvht.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/libcvht_wrap.c` & `vht-0.3.96/libvht/libcvht_wrap.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/libvht.c` & `vht-0.3.96/libvht/libvht.c`

 * *Files 16% similar despite different names*

```diff
@@ -22,53 +22,18 @@
 #include "jack_process.h"
 
 #include "module.h"
 
 // getters/setters and stuff for python
 
 // dear mother of god...
-inline void trk_should_save(track *trk) {
-	if (trk->clt) {
-		midi_client *clt = (midi_client *)trk->clt;
-		module *mod = (module *)clt->mod_ref;
-		mod->should_save = 1;
-	}
-}
-
-inline void seq_should_save(sequence *seq) {
-	if (seq->clt) {
-		midi_client *clt = (midi_client *)seq->clt;
-		module *mod = (module *)clt->mod_ref;
-		mod->should_save = 1;
-	}
-}
-
-inline void mod_should_save(module *mod) {
-	if (mod->clt) {
-		midi_client *clt = (midi_client *)mod->clt;
-		module *mod = (module *)clt->mod_ref;
-		mod->should_save = 1;
-	}
-}
-
-inline void tl_should_save(timeline *tl) {
-	if (tl->clt) {
-		midi_client *clt = (midi_client *)tl->clt;
-		module *mod = (module *)clt->mod_ref;
-		mod->should_save = 1;
-	}
-}
-
-inline void ts_should_save(timestrip *ts) {
-	if (ts->seq->clt) {
-		midi_client *clt = (midi_client *)ts->seq->clt;
-		module *mod = (module *)clt->mod_ref;
-		mod->should_save = 1;
-	}
-}
+void trk_should_save(track *trk);
+void ts_should_save(timestrip *ts);
+void tl_should_save(timeline *tl);
+void seq_should_save(sequence *seq);
 
 int charpp_nitems(char **cpp) {
 	if (!cpp)
 		return 0;
 
 	int p = 0;
 	while(cpp[p++]);
```

### Comparing `vht-0.3.69/libvht/mandy.c` & `vht-0.3.96/libvht/mandy.c`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 	tracy_del(mand->init_trc);
 	free(mand->pix_mask);
 	pthread_mutex_destroy(&mand->excl);
 	pthread_mutex_destroy(&mand->excl_vect);
 	free(mand);
 }
 
-inline double rad2deg(double r) {
+double rad2deg(double r) {
 	double deg = r * (180.0 / M_PI);
 	while(deg < -180.0)
 		deg += 360.0;
 
 	while(deg > 180.0)
 		deg -= 360.0;
 
@@ -566,15 +566,15 @@
 		mand->y = dy;
 		mand->rot = drot;
 		mand->zoom = dzoom;
 	}
 }
 
 // the algo
-inline unsigned char mandy_v(mandy *mand, long double x, long double y) {
+unsigned char mandy_v(mandy *mand, long double x, long double y) {
 	long double xx = mand->jx;
 	long double yy = mand->jy;
 	long double nx = 0.0;
 	long double ny = 0.0;
 	long double sx = x;
 	long double sy = y;
 	unsigned char v = 0;
```

### Comparing `vht-0.3.69/libvht/mandy.h` & `vht-0.3.96/libvht/mandy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/mandy_pix_scan.c` & `vht-0.3.96/libvht/mandy_pix_scan.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/mandy_pix_scan.h` & `vht-0.3.96/libvht/mandy_pix_scan.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/mandy_trk_disp.c` & `vht-0.3.96/libvht/mandy_trk_disp.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/mandy_trk_disp.h` & `vht-0.3.96/libvht/mandy_trk_disp.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/midi_client.c` & `vht-0.3.96/libvht/midi_client.c`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	clt->jack_sample_rate = 0;
 	clt->jack_buffer_size = 0;
 	clt->jack_last_frame = 0;
 	clt->error = NULL;
 	clt->default_midi_port = 0;
 	clt->mod_ref = mod;
 	clt->running = 0;
+	clt->freewheeling = 0;
 	clt->dump_notes = 0;
 	clt->ports = 0;
 	clt->ports_changed = 0;
 	clt->jack_client_name = 0;
 
 	for (int p = 0; p < MIDI_CLIENT_MAX_PORTS; p++) {
 		clt->ports_to_open[p] = 0;
@@ -687,10 +688,10 @@
 }
 
 int get_default_midi_out_port(midi_client *clt) {
 	return clt->default_midi_port;
 }
 
 void midi_set_freewheel(midi_client *clt, int on) {
-	//printf("freewheel %d\n", on);
+	clt->freewheeling = on;
 	jack_set_freewheel(clt->jack_client, on);
 }
```

### Comparing `vht-0.3.69/libvht/midi_client.h` & `vht-0.3.96/libvht/midi_client.h`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 - have fun! */
 
 typedef struct midi_client_t {
 	void *mod_ref;
 	int default_midi_port;
 	char *error;
 	int running;
+	int freewheeling;
 	int dump_notes;
 
 	jack_client_t *jack_client;
 	jack_port_t *jack_input_port;
 	int ports_to_open[MIDI_CLIENT_MAX_PORTS];
 	int autoports[MIDI_CLIENT_MAX_PORTS];
```

### Comparing `vht-0.3.69/libvht/midi_event.c` & `vht-0.3.96/libvht/midi_event.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/midi_event.h` & `vht-0.3.96/libvht/midi_event.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/module.c` & `vht-0.3.96/libvht/module.c`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 	pthread_mutex_lock(&mod->excl);
 }
 
 void module_excl_out(module *mod) {
 	pthread_mutex_unlock(&mod->excl);
 }
 
-inline void mod_should_save(module *mod) {
+void mod_should_save(module *mod) {
 	mod->should_save = 1;
 }
 
-inline void module_handle_inception(track *trk, midi_event evt) {
+void module_handle_inception(track *trk, midi_event evt) {
 	midi_client *clt = (midi_client *)trk->clt;
 	module *mod = (module *)clt->mod_ref;
 
 	if (mod->inception && trk->port == 15) {
 		for (int s = 0; s < mod->nseq; s++)
 			sequence_handle_trigger_event(mod->seq[s], evt);
 	}
```

### Comparing `vht-0.3.69/libvht/module.h` & `vht-0.3.96/libvht/module.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/row.c` & `vht-0.3.96/libvht/row.c`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  */
 
 #include <stdlib.h>
 #include "row.h"
 #include "midi_client.h"
 #include "module.h"
 
-inline void rw_should_save(row *rw) {
+void rw_should_save(row *rw) {
 	if (rw->clt) {
 		midi_client *clt = (midi_client *)rw->clt;
 		module *mod = (module *)clt->mod_ref;
 		mod->should_save = 1;
 	}
 }
 int row_get_type(row *rw) {
```

### Comparing `vht-0.3.69/libvht/row.h` & `vht-0.3.96/libvht/row.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/sequence.c` & `vht-0.3.96/libvht/sequence.c`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 }
 
 void seq_mod_excl_out(sequence *seq) {
 	if (seq->mod_excl)
 		pthread_mutex_unlock(seq->mod_excl);
 }
 
-inline void seq_should_save(sequence *seq) {
+void seq_should_save(sequence *seq) {
 	if (seq->clt) {
 		midi_client *clt = (midi_client *)seq->clt;
 		module *mod = (module *)clt->mod_ref;
 		mod->should_save = 1;
 	}
 }
```

### Comparing `vht-0.3.69/libvht/sequence.h` & `vht-0.3.96/libvht/sequence.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #define __SEQUENCE_H__
 #include <pthread.h>
 #include <semaphore.h>
 #include "midi_event.h"
 #include "track.h"
 
 
-#define SEQUENCE_MAX_LENGTH	512
+#define SEQUENCE_MAX_LENGTH	1024
 
 #define PLAY_TRIGGER_ONOFF		0
 #define PLAY_TRIGGER_ONESHOT	1
 #define PLAY_TRIGGER_HOLD		2
 
 #define TRIGGER_MUTE			0
 #define TRIGGER_CUE				1
```

### Comparing `vht-0.3.69/libvht/smf.c` & `vht-0.3.96/libvht/smf.c`

 * *Files 2% similar despite different names*

```diff
@@ -93,22 +93,24 @@
 			for (int tt = 0; tt < mod->seq[s]->ntrk; tt++) {
 				track *trk = mod->seq[s]->trk[tt];
 
 				if ((trk->channel == evt.channel) && (trk->port == port)) {
 					char *b;
 					char *xtr = track_get_extras(trk);
 
-					b = strstr(xtr, "\"track_name\": \"");
-					if (b) {
-						b+=15;
-						char *bb = strstr(b, "\"");
-						int l = bb - b;
-						if (l > 0) {
-							strncpy(mf->trk_inf[t].name, b, l);
-							mf->trk_inf[t].name[l] = 0;
+					if (xtr) {
+						b = strstr(xtr, "\"track_name\": \"");
+						if (b) {
+							b+=15;
+							char *bb = strstr(b, "\"");
+							int l = bb - b;
+							if (l > 0) {
+								strncpy(mf->trk_inf[t].name, b, l);
+								mf->trk_inf[t].name[l] = 0;
+							}
 						}
 					}
 				}
 			}
 		}
 
 		found = t;
@@ -216,15 +218,15 @@
 		qsort(mf->trk_inf[t].evts, mf->trk_inf[t].nevt, sizeof(evthist), comp_evts);
 
 		// dump track
 		smf_push_str(mf, "MTrk");
 		loffs = mf->bin_l;
 		smf_push_long(mf, 0);
 		// name
-		if (mf->trk_inf[t].name) {
+		if (mf->trk_inf[t].name[0]) {
 			smf_push(mf, 0);
 			smf_push_short(mf, 0xff03);
 			smf_push(mf, strlen(mf->trk_inf[t].name));
 			smf_push_str(mf, mf->trk_inf[t].name);
 		}
 
 		// channel
```

### Comparing `vht-0.3.69/libvht/smf.h` & `vht-0.3.96/libvht/smf.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/stolen.c` & `vht-0.3.96/libvht/stolen.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/timeline.c` & `vht-0.3.96/libvht/timeline.c`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,23 @@
 	pthread_mutex_lock(&tl->excl);
 }
 
 void timeline_excl_out(timeline *tl) {
 	pthread_mutex_unlock(&tl->excl);
 }
 
-inline void tl_should_save(timeline *tl) {
+void ts_should_save(timestrip *ts) {
+	if (ts->seq->clt) {
+		midi_client *clt = (midi_client *)ts->seq->clt;
+		module *mod = (module *)clt->mod_ref;
+		mod->should_save = 1;
+	}
+}
+
+void tl_should_save(timeline *tl) {
 	if (tl->clt) {
 		midi_client *clt = (midi_client *)tl->clt;
 		module *mod = (module *)clt->mod_ref;
 		mod->should_save = 1;
 	}
 }
```

### Comparing `vht-0.3.69/libvht/timeline.h` & `vht-0.3.96/libvht/timeline.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/track.c` & `vht-0.3.96/libvht/track.c`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 #include <math.h>
 
 #include "midi_client.h"
 #include "module.h"
 #include "track.h"
 #include "row.h"
 
-inline void trk_mod_excl_in(track *trk) {
+void trk_mod_excl_in(track *trk) {
 	if (trk->mod_excl)
 		pthread_mutex_lock(trk->mod_excl);
 }
 
-inline void trk_mod_excl_out(track *trk) {
+void trk_mod_excl_out(track *trk) {
 	if (trk->mod_excl)
 		pthread_mutex_unlock(trk->mod_excl);
 }
 
-inline void trk_should_save(track *trk) {
+void trk_should_save(track *trk) {
 	if (trk->clt) {
 		midi_client *clt = (midi_client *)trk->clt;
 		module *mod = (module *)clt->mod_ref;
 		mod->should_save = 1;
 	}
 }
```

### Comparing `vht-0.3.69/libvht/track.h` & `vht-0.3.96/libvht/track.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/tracy.c` & `vht-0.3.96/libvht/tracy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/tracy.h` & `vht-0.3.96/libvht/tracy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtcolumn.py` & `vht-0.3.96/libvht/vhtcolumn.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtctrl.py` & `vht-0.3.96/libvht/vhtctrl.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtctrllist.py` & `vht-0.3.96/libvht/vhtctrllist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtctrlrow.py` & `vht-0.3.96/libvht/vhtctrlrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtextras.py` & `vht-0.3.96/libvht/vhtextras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtmandy.py` & `vht-0.3.96/libvht/vhtmandy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtmodule.py` & `vht-0.3.96/libvht/vhtmodule.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtport.py` & `vht-0.3.96/libvht/vhtport.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtports.py` & `vht-0.3.96/libvht/vhtports.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtquicklist.py` & `vht-0.3.96/libvht/vhtquicklist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtrow.py` & `vht-0.3.96/libvht/vhtrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhtsequence.py` & `vht-0.3.96/libvht/vhtsequence.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimeline.py` & `vht-0.3.96/libvht/vhttimeline.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelinechange.py` & `vht-0.3.96/libvht/vhttimelinechange.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelinechanges.py` & `vht-0.3.96/libvht/vhttimelinechanges.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelineloop.py` & `vht-0.3.96/libvht/vhttimelineloop.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelineslices.py` & `vht-0.3.96/libvht/vhttimelineslices.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelinestrip.py` & `vht-0.3.96/libvht/vhttimelinestrip.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelinestrips.py` & `vht-0.3.96/libvht/vhttimelinestrips.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttimelineticks.py` & `vht-0.3.96/libvht/vhttimelineticks.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttrack.py` & `vht-0.3.96/libvht/vhttrack.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/libvht/vhttracy.py` & `vht-0.3.96/libvht/vhttracy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/pyproject.toml` & `vht-0.3.96/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
 build-backend = 'setuptools.build_meta'
 requires = ["setuptools>=61.0"]
-
 [metadata]
 name = "vht"
-version = "0.3.69"
-description = "vahatraker - a live MIDI sequencer for JACK"
+version = "0.3.96"
+description = "vahatraker - a live MIDI sequencer for pipewire/JACK"
 author = "Remigiusz Dybka"
 author_email = "remigiusz.dybka@gmail.com"
 url = "https://github.com/rdybka/vht"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -35,17 +34,18 @@
 [options.package_data]
 vht = ["data/*", "data/ctrl/*", "data/bank/*"]
 
 [options.data_files]
 "share/vht" = ["data/mandy.png", "data/vht.svg", "data/vht.png", "data/menu.ui"]
 "share/vht/ctrl" = ["data/ctrl/10-gm", "data/ctrl/20-zyn"]
 "share/vht/bank" = ["data/bank/10-gm1", "data/bank/20-gm2"]
-"share/icons" = ["data/vht.svg"]
+"share/icons/hicolor/scalable" = ["data/net.sourceforge.projects.vht.svg"]
 "share/man/man1" = ["doc/vht.1.gz"]
-"share/applications" = ["data/com.github.rdybka.vht.desktop"]
+"share/applications" = ["data/net.sourceforge.projects.vht.desktop"]
+"share/metainfo" = ["data/net.sourceforge.projects.vht.metainfo.xml"]
 
 [options.extensions]
 "libvht/_libcvht" = ["libvht/libvht.c", 
 "libvht/libcvht_wrap.c",
 "libvht/midi_client.c",
 "libvht/jack_process.c",
 "libvht/midi_event.c",
```

### Comparing `vht-0.3.69/setup.py` & `vht-0.3.96/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name = "vht",
-	version = "0.3.69",
-	description = "vahatraker - a live MIDI sequencer for JACK",
+	version = "0.3.96",
+	description = "vahatraker - a live MIDI sequencer for pipewire/JACK",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "Remigiusz Dybka",
 	author_email = "remigiusz.dybka@gmail.com",
 	url = "https://github.com/rdybka/vht",
 	license = 'GPLv3+',
 	ext_modules = [Extension("libvht/_libcvht", ["libvht/libvht.c",
@@ -40,17 +40,18 @@
 		'vht = vht.main:run',
 		]},
 	
 	data_files = [
 		('share/vht', ['data/mandy.png', 'data/vht.svg', 'data/vht.png', 'data/menu.ui']),
 		('share/vht/ctrl', ['data/ctrl/10-gm', 'data/ctrl/20-zyn']),
 		('share/vht/bank', ['data/bank/10-gm1', 'data/bank/20-gm2']),
-		('share/icons', ['data/vht.svg']),
+		('share/icons/hicolor/scalable/apps', ['data/net.sourceforge.projects.vht.svg']),
 		('share/man/man1', ['doc/vht.1.gz']),
-		('share/applications', ['data/com.github.rdybka.vht.desktop'])
+		('share/applications', ['data/net.sourceforge.projects.vht.desktop']),
+		('share/metainfo' , ['data/net.sourceforge.projects.vht.metainfo.xml'])
 		
 	],
 	
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: X11 Applications :: GTK',
 		'Intended Audience :: End Users/Desktop',
```

### Comparing `vht-0.3.69/vht/autoexec.py` & `vht-0.3.96/vht/autoexec.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/bankcfg.py` & `vht-0.3.96/vht/bankcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/capturebutton.py` & `vht-0.3.96/vht/capturebutton.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/codedaemon.py` & `vht-0.3.96/vht/codedaemon.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/configuration.py` & `vht-0.3.96/vht/configuration.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/console.py` & `vht-0.3.96/vht/console.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/controllereditor.py` & `vht-0.3.96/vht/controllereditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/controllersview.py` & `vht-0.3.96/vht/controllersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/controllersviewrow.py` & `vht-0.3.96/vht/controllersviewrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,11 +153,11 @@
             self.entry.set_text(n[c])
         else:
             self.entry.set_text("")
 
         self.parent.ctrl_names[str(self.index)] = (self.parn, self.entry.get_text())
         self.parent.trk.extras.write()
         self.trk.ctrl[self.index].ctrlnum = self.ctrlnum
-        self.parent.trkview.controller_editors[
-            self.index - 1
-        ].midi_ctrlnum = self.ctrlnum
+        self.parent.trkview.controller_editors[self.index - 1].midi_ctrlnum = (
+            self.ctrlnum
+        )
         self.parent.rebuild()
```

### Comparing `vht-0.3.69/vht/controllerundobuffer.py` & `vht-0.3.96/vht/controllerundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/ctrlcfg.py` & `vht-0.3.96/vht/ctrlcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/extras.py` & `vht-0.3.96/vht/extras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/filerotator.py` & `vht-0.3.96/vht/filerotator.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/main.py` & `vht-0.3.96/vht/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # I hereby testify,
-# on Boomtime, the 9th day of Discord in the YOLD 3189,
+# on Pungenday, the 2nd day of Confusion in the YOLD 3190,
 # that everything in this program checks out with The Law of Fives
 
 # [^^^intentionally left blank]
 
 import gi
 
 gi.require_version("Gtk", "3.0")
@@ -44,15 +44,15 @@
 import vht.filerotator
 
 
 class VHTApp(Gtk.Application):
     def __init__(self, *args, **kwargs):
         super().__init__(
             *args,
-            application_id="com.github.rdybka.vht",
+            application_id="net.sourceforge.projects.vht",
             flags=Gio.ApplicationFlags.HANDLES_OPEN | Gio.ApplicationFlags.NON_UNIQUE,
             **kwargs
         )
 
         self.main_win = None
         self.start_load_file = None
 
@@ -204,15 +204,15 @@
         ab.set_license_type(Gtk.License.GPL_3_0)
         ab.set_copyright(
             "Copyright (C) 2024 Remigiusz Dybka\nremigiusz.dybka@gmail.com"
         )
         pkg = pkg_resources.require("vht")[0]
         ab.set_version(pkg.version)
         ab.set_program_name("vahatraker")
-        ab.set_comments("a live MIDI sequencer for JACK")
+        ab.set_comments("a live MIDI sequencer for pipewire/JACK")
         ab.set_logo(
             GdkPixbuf.Pixbuf.new_from_file_at_size(
                 mod.data_path + os.sep + "vht.svg", 160, 160
             )
         )
 
         ab.run()
```

### Comparing `vht-0.3.69/vht/mainwin.py` & `vht-0.3.96/vht/mainwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from vht.console import Console
 from vht.sequencelistview import SequenceListView
 from vht.timelineview import TimelineView
 from vht.statusbar import StatusBar
 from vht.sequenceview import SequenceView
 from vht.thumbmanager import ThumbManager
 from vht.renderer import Renderer
 from vht.portconfig import *
@@ -29,17 +28,23 @@
 from vht import *
 import vht.extras
 
 import gi
 import os
 
 gi.require_version("Gtk", "3.0")
-gi.require_version("Vte", "2.91")
+
 from gi.repository import Gtk, Gdk, Gio
 
+try:
+    gi.require_version("Vte", "2.91")
+    from vht.console import Console
+except Exception:
+    Console = None
+
 
 class MainWin(Gtk.ApplicationWindow):
     def __init__(self, app):
         super(MainWin, self).__init__(application=app)
         # here we GUI
 
         self.fs = False
@@ -128,15 +133,18 @@
 
         self.sequence_view = SequenceView(mod[mod.curr_seq])
         self.hbox.set_orientation(Gtk.Orientation.HORIZONTAL)
 
         self.seqbox.pack1(self.sequence_view, True, True)
 
         self.hbox.pack1(self.seqbox, True, True)
-        self.console = Console()
+        if Console:
+            self.console = Console()
+        else:
+            self.console = None
 
         self.timeline_box = Gtk.Paned()
         self.timeline_box.set_orientation(Gtk.Orientation.VERTICAL)
         self.timeline_box.set_wide_handle(True)
 
         self.seqlist = SequenceListView()
         mod.seqlist = self.seqlist
@@ -358,22 +366,28 @@
 
         self.hbox.set_wide_handle(True)
         self.timeline_visible = True
         self.timeline_box.show_all()
         cfg.timeline_show = True
 
     def hide_console(self):
+        if not Console:
+            return
+
         if not mod.console_visible:
             return
 
         self.console.hide()
         mod.console_visible = False
         self.sequence_view.auto_scroll_req = True
 
     def show_console(self):
+        if not Console:
+            return
+
         if mod.console_visible:
             return
 
         if 1 == len(self.seqbox.get_children()):
             self.seqbox.pack2(self.console, True, True)
             self.seqbox.set_position(
                 self.get_window().get_height() * cfg.console_position
```

### Comparing `vht-0.3.69/vht/mandymenu.py` & `vht-0.3.96/vht/mandymenu.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/mandyview.py` & `vht-0.3.96/vht/mandyview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/midimapview.py` & `vht-0.3.96/vht/midimapview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/midimapviewrow.py` & `vht-0.3.96/vht/midimapviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/notebooklabel.py` & `vht-0.3.96/vht/notebooklabel.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/poormanspiano.py` & `vht-0.3.96/vht/poormanspiano.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/portconfig.py` & `vht-0.3.96/vht/portconfig.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/portconfigpopover.py` & `vht-0.3.96/vht/portconfigpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/portconfigview.py` & `vht-0.3.96/vht/portconfigview.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,21 @@
 
         self.insert(self.head_row, 0)
         wdg = self.get_children()[0]
         wdg.set_sensitive(False)
 
     def add(self, prtname, pretty, state):
         rw = Gtk.Box()
-        rw.pack_start(Gtk.Label(pretty if pretty else prtname), False, False, 0)
+        lb = Gtk.Label(prtname[:33])
+        if pretty:
+            lb.set_tooltip_markup(
+                """<span font_family="Monospace" size="medium">%s</span>""" % (pretty)
+            )
+
+        rw.pack_start(lb, False, False, 0)
         statewdg = Gtk.CheckButton()
         statewdg.set_active(state)
         statewdg.connect("toggled", self.tgl_meta, prtname)
         rw.pack_end(statewdg, False, False, 0)
         self.insert(rw, -1)
 
     def tgl_meta(self, widget, prtname):
```

### Comparing `vht-0.3.69/vht/preferenceswin.py` & `vht-0.3.96/vht/preferenceswin.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,58 +239,58 @@
         grid.set_margin_top(mrg)
         grid.set_margin_bottom(mrg)
         grid.set_margin_left(mrg)
         grid.set_margin_right(mrg)
 
         fr, gr = self.create_frame("Default input", mrg)
         cmb = Gtk.ComboBoxText()
-        cmb.set_hexpand(True)
+        cmb.set_hexpand(False)
         cmb.append_text("none")
         pp = []
         pretty = {}
         for prt in self.mod.ports:
             if prt.type == "midi" and not prt.mine and prt.output:
                 pp.append(prt.name)
                 pretty[prt.name] = prt.pname
 
         dinp = self.cfg.midi_default_input
         if dinp and dinp not in pp:
             pp.append(dinp)
 
         for prt in pp:
-            cmb.append(prt, pretty[prt] if prt in pretty else prt)
+            cmb.append(prt, pretty[prt][:33] if prt in pretty else prt)
 
         dinp = self.cfg.midi_default_input
         if dinp and dinp in pp:
             cmb.set_active(pp.index(dinp) + 1)
         else:
             cmb.set_active(0)
 
         self.midi_in_cmb = cmb
         gr.attach(cmb, 0, 0, 1, 1)
         grid.attach(fr, 0, 0, 1, 1)
 
         fr, gr = self.create_frame("Default output", mrg)
         cmb = Gtk.ComboBoxText()
-        cmb.set_hexpand(True)
+        cmb.set_hexpand(False)
         cmb.append_text("none")
 
         pp = []
         pretty = {}
         for prt in self.mod.ports:
             if prt.type == "midi" and not prt.mine and prt.input:
                 pp.append(prt.name)
                 pretty[prt.name] = prt.pname
 
         doutp = self.cfg.midi_default_output
         if doutp and doutp not in pp:
             pp.append(doutp)
 
         for prt in pp:
-            cmb.append(prt, pretty[prt] if prt in pretty else prt)
+            cmb.append(prt, pretty[prt][:33] if prt in pretty else prt)
 
         doutp = self.cfg.midi_default_output
         if doutp and doutp in pp:
             cmb.set_active(pp.index(doutp) + 1)
         else:
             cmb.set_active(0)
```

### Comparing `vht-0.3.69/vht/probeditor.py` & `vht-0.3.96/vht/probeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/propview.py` & `vht-0.3.96/vht/propview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/pulsar.py` & `vht-0.3.96/vht/pulsar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/randomcomposer.py` & `vht-0.3.96/vht/randomcomposer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/renderer.py` & `vht-0.3.96/vht/renderer.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,15 +134,14 @@
         self._finished = False
 
     def start_wudh(self, folder, filename, fmt, meter):
         self._finished = False
 
         opts = ["jack_capture"]
         opts.append("-jf")
-        # opts.append("--daemon")
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + "_"))
         if self.cfg.render_midi:
             self._midi_file = os.path.join(folder, filename + ".mid")
         else:
@@ -168,31 +167,30 @@
         folder = self._qopts[0]
         filename = self._qopts[1]
         fmt = self._qopts[2]
         lead_out = self._qopts[3]
 
         opts = ["jack_capture"]
         opts.append("-jf")
-        # opts.append("--daemon")
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + ("_seq%02d" % seqid) + "_"))
         if self.cfg.render_midi:
             self._midi_file = os.path.join(folder, filename + ("_seq%02d.mid" % seqid))
 
         self.mod.play = 0
         self.mod.reset()
         self.mod.reset()  # in case some old note-offs hang
         for s in self.mod:
             s.playing = False
 
-        self.mod.play_mode = 0
         self.mod.render_mode = 1
         self._orig_pm = self.mod.play_mode
+        self.mod.play_mode = 0
         self.mod.set_lead_out(lead_out)
 
         for m in self.mod:
             if m.index == seqid:
                 m.playing = 1
             else:
                 m.playing = 0
@@ -223,15 +221,14 @@
             self._finished = True
 
     def start_timeline(self, folder, filename, fmt, lead_out):
         self._finished = False
 
         opts = ["jack_capture"]
         opts.append("-jf")
-        # opts.append("--daemon")
         opts.append("-f")
         opts.append(fmt)
         opts.append("-fp")
         opts.append(os.path.join(folder, filename + "_"))
         if self.cfg.render_midi:
             self._midi_file = os.path.join(folder, filename + ".mid")
         else:
```

### Comparing `vht-0.3.69/vht/renderwin.py` & `vht-0.3.96/vht/renderwin.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from gi.repository import GLib, Gtk, Gdk
 
 
 class RenderWin(Gtk.Window):
     def __init__(self, parent, mod, cfg):
         super(RenderWin, self).__init__()
+
         self.cfg = cfg
         self.mod = mod
         self.parent = parent
         self.mod.render_win_showing = True
         self.allow_exit = True
         self.capturing = False
         self.rend = mod.renderer
```

### Comparing `vht-0.3.69/vht/sequencelistview.py` & `vht-0.3.96/vht/sequencelistview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/sequencelistviewpopover.py` & `vht-0.3.96/vht/sequencelistviewpopover.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,22 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import copy
 import gi
 
 gi.require_version("Gtk", "3.0")
-gi.require_version("GtkSource", "4")
 
-from gi.repository import Gdk, Gtk, Gio, GtkSource
+from gi.repository import Gdk, Gtk, Gio
+
+try:
+    gi.require_version("GtkSource", "4")
+    from gi.repository import GtkSource
+except Exception:
+    GtkSource = None
 
 from vht.notebooklabel import NotebookLabel
 from vht.sequencetriggersview import SequenceTriggersView
 from vht.controllersview import ControllersView
 from vht import cfg, mod, extras
 from datetime import datetime
 from vht.poormanspiano import PoorMansPiano
@@ -90,51 +95,56 @@
         grid2.attach(box, 0, 1, 3, 1)
 
         self._trgview = SequenceTriggersView(-1, self)
         grid.attach(self._trgview, 0, 1, 3, 1)
 
         self._code_butt = Gtk.ToggleButton()
         self._code_butt.set_active(False)
+
         icon = Gio.ThemedIcon(name="system-run")
         image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
         self._code_butt.add(image)
         self._code_butt.connect("clicked", self.on_code_butt_toggled)
-        box.pack_end(self._code_butt, False, False, 2)
+        if GtkSource:
+            box.pack_end(self._code_butt, False, False, 2)
+
         # self._trgview.attach(self._code_butt, 0, 3, 1, 1)
 
         self._run_switch = Gtk.Switch()
         self._run_switch.set_state(False)
         self._run_switch.connect("state-set", self.on_run_switch)
 
-        self._err_butt = Gtk.Button.new_with_label("err")
-        self._err_butt.connect("clicked", self.on_err_butt_clicked)
+        if GtkSource:
+            self._err_butt = Gtk.Button.new_with_label("err")
+            self._err_butt.connect("clicked", self.on_err_butt_clicked)
 
-        box.pack_end(self._err_butt, False, False, 2)
-        box.pack_end(self._run_switch, False, False, 2)
+            box.pack_end(self._err_butt, False, False, 2)
+            box.pack_end(self._run_switch, False, False, 2)
 
         box.pack_end(self._entry, True, True, 2)
         # self._trgview.attach(self._run_switch, 5, 3, 1, 1)
 
-        self._textview = GtkSource.View()  # .GtkSourceView()
-        self._textview.set_monospace(True)
-        self._textview.set_tab_width(4)
-        self._textview.set_indent_width(4)
-        self._textview.set_indent_on_tab(True)
-        self._textview.set_show_line_numbers(True)
-        self._textview.set_auto_indent(True)
-        self._textview.set_smart_backspace(True)
-        self._textview.set_insert_spaces_instead_of_tabs(True)
-        tb = self._textview.get_buffer()
-        tb.connect("changed", self.on_tb_changed)
-
-        self._scroll = Gtk.ScrolledWindow()
-        self._scroll.add(self._textview)
-        grid.attach(self._scroll, 0, 2, 3, 2)
+        if GtkSource:
+            self._textview = GtkSource.View()
+            self._textview.set_monospace(True)
+            self._textview.set_tab_width(4)
+            self._textview.set_indent_width(4)
+            self._textview.set_indent_on_tab(True)
+            self._textview.set_show_line_numbers(True)
+            self._textview.set_auto_indent(True)
+            self._textview.set_smart_backspace(True)
+            self._textview.set_insert_spaces_instead_of_tabs(True)
+            tb = self._textview.get_buffer()
+            tb.connect("changed", self.on_tb_changed)
+
+            self._scroll = Gtk.ScrolledWindow()
+            self._scroll.add(self._textview)
+            grid.attach(self._scroll, 0, 2, 3, 2)
 
-        self._scrollgrid = grid
+            self._scrollgrid = grid
 
         grid2.attach(grid, 0, 0, 3, 1)
 
         grid2.show_all()
         self.add(grid2)
         self.set_modal(False)
         self.pooped = False
@@ -160,25 +170,31 @@
         if cpt > -1:
             mnt = self.pmp.k2n(event.keyval)
             if mnt > -1:
                 mod[tv.seq].set_trig(cpt, 1, 1, mnt)
                 tv.refresh()
 
     def hide_code(self):
+        if not GtkSource:
+            return
+
         buff = self._textview.get_buffer()
         buff.set_text("")
         if self._scroll in self._scrollgrid:
             self._scrollgrid.remove(self._scroll)
         self._run_switch.set_state(False)
         self._run_switch.set_sensitive(False)
         self._run_switch.set_visible(False)
         self._err_butt.set_visible(False)
         self._code_butt.set_active(False)
 
     def show_code(self):
+        if not GtkSource:
+            return
+
         if not self._scroll in self._scrollgrid:
             self._scrollgrid.attach(self._scroll, 0, 2, 3, 2)
 
         self._run_switch.set_sensitive(True)
         self._run_switch.set_visible(True)
 
         self._code_butt.set_active(True)
@@ -246,15 +262,15 @@
 
         if self.time_want_to_leave == -2:
             return True
 
         if self.time_want_to_leave == -1:  # closed - stop callback
             return False
 
-        if self._scroll in self._scrollgrid:
+        if GtkSource and self._scroll in self._scrollgrid:
             self.time_want_to_leave = 0
             return True
 
         if self._trgview.play_mode_cb.props.popup_shown:
             self.time_want_to_leave = 0
             return True
```

### Comparing `vht-0.3.69/vht/sequencepropviewpopover.py` & `vht-0.3.96/vht/sequencepropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/sequencetriggersview.py` & `vht-0.3.96/vht/sequencetriggersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/sequenceview.py` & `vht-0.3.96/vht/sequenceview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/shortcutmayhem.py` & `vht-0.3.96/vht/shortcutmayhem.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from vht import *
 import vht.extras
 
 import gi
 import os
 
 gi.require_version("Gtk", "3.0")
-gi.require_version("Vte", "2.91")
 from gi.repository import Gtk, Gdk
 
 
 def shrt(grp, ttl, k):
     itm = Gtk.ShortcutsShortcut(title=ttl, accelerator=cfg.key[k].to_accel())
     itm.show()
     grp.add(itm)
```

### Comparing `vht-0.3.69/vht/sidetrackview.py` & `vht-0.3.96/vht/sidetrackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/statusbar.py` & `vht-0.3.96/vht/statusbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,21 +394,24 @@
             if self.active_field == 3:  # skip
                 self.tt_txt = "<big>↑</big> %s\n<big>↓</big> %s" % (
                     cfg.key["skip_up"],
                     cfg.key["skip_down"],
                 )
 
             if self.active_field == 4:  # bpm
-                self.tt_txt = "<big> ⇑</big> %s\n<big> ↑</big> %s\n<big>.↑</big> %s\n<big>.↓</big> %s\n<big> ↓</big> %s\n<big> ⇓</big> %s" % (
-                    cfg.key["bpm_10_up"],
-                    cfg.key["bpm_up"],
-                    cfg.key["bpm_frac_up"],
-                    cfg.key["bpm_frac_down"],
-                    cfg.key["bpm_down"],
-                    cfg.key["bpm_10_down"],
+                self.tt_txt = (
+                    "<big> ⇑</big> %s\n<big> ↑</big> %s\n<big>.↑</big> %s\n<big>.↓</big> %s\n<big> ↓</big> %s\n<big> ⇓</big> %s"
+                    % (
+                        cfg.key["bpm_10_up"],
+                        cfg.key["bpm_up"],
+                        cfg.key["bpm_frac_up"],
+                        cfg.key["bpm_frac_down"],
+                        cfg.key["bpm_down"],
+                        cfg.key["bpm_10_down"],
+                    )
                 )
 
             if self.active_field == 5:  # rpb
                 self.tt_txt = "<big>↑</big> %s\n<big>↓</big> %s" % (
                     cfg.key["rpb_up"],
                     cfg.key["rpb_down"],
                 )
```

### Comparing `vht-0.3.69/vht/thumbmanager.py` & `vht-0.3.96/vht/thumbmanager.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/timelineview.py` & `vht-0.3.96/vht/timelineview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/timeshifteditor.py` & `vht-0.3.96/vht/timeshifteditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/trackpropview.py` & `vht-0.3.96/vht/trackpropview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/trackpropviewpopover.py` & `vht-0.3.96/vht/trackpropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/trackundobuffer.py` & `vht-0.3.96/vht/trackundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/trackview.py` & `vht-0.3.96/vht/trackview.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         self.drag = False
         self.sel_drag = False
         self.sel_dragged = False
         self.sel_drag_prev = None
         self.sel_drag_back = None
         self.sel_drag_front = None
         self.sel_drag_start = 0
+        self.drag_cloned = False
         self.select = False
         self.select_start = None
         self.select_end = None
 
         self.nudge_last_y = -1
         self.nudge_hide_timeshift = False
         self.nudge_buff = None
@@ -925,15 +926,15 @@
         if event.x < self.txt_width * len(self.trk):
             if self.keyboard_focus:
                 if self.keyboard_focus.edit == -1:
                     self.keyboard_focus = None
 
                 if self.keyboard_focus:
                     if self.keyboard_focus.selection:
-                        self.keyboard_focus = None
+                        return
 
         if self.show_pitchwheel:
             self.pitchwheel_editor.on_motion(widget, event)
 
         if self.show_controllers:
             for ctrl in self.controller_editors:
                 ctrl.on_motion(ctrl, event)
@@ -1062,17 +1063,23 @@
         if self.drag:
             self.parent.autoscroll_req = True
             if (
                 self.trk[new_hover_column][new_hover_row].type == 0
             ):  # dragging single cell
                 if self.edit[1] != new_hover_row or self.edit[0] != new_hover_column:
                     old_row = self.edit[1]
+                    olr = self.trk[self.edit[0]][self.edit[1]]
                     self.swap_row(
                         self.edit[0], self.edit[1], new_hover_column, new_hover_row
                     )
+
+                    if self.drag_cloned:
+                        olr.copy(self.trk[new_hover_column][new_hover_row])
+                        self.drag_cloned = False
+
                     self.edit = new_hover_column, new_hover_row
 
                     self.redraw(new_hover_row)
                     self.redraw(old_row)
 
         if self.sel_drag:  # dragging selection
             dx = new_hover_column - self.sel_drag_prev[0]
@@ -1311,17 +1318,14 @@
             return True
 
         enter_edit = False
 
         if event.button != cfg.select_button and event.button != 2:
             return False
 
-        if event.state & Gdk.ModifierType.CONTROL_MASK:
-            return False
-
         if row >= self.trk.nrows:
             return False
 
         self.sel_drag = False
         self.sel_dragged = False
         if event.button == cfg.select_button:
             if self.select_start:
@@ -1357,14 +1361,20 @@
                     self.select_start = None
                     self.select_end = None
 
             if self.trk[col][row].type in (1, 2):  # note_on
                 enter_edit = True
                 self.drag = True
 
+                if event.state & Gdk.ModifierType.CONTROL_MASK:
+                    self.drag_cloned = True
+        else:
+            if event.state & Gdk.ModifierType.CONTROL_MASK:
+                return False
+
         flds = 2
         if self.show_timeshift:
             flds += 1
 
         if self.show_probs:
             flds += 1
 
@@ -1491,18 +1501,17 @@
 
                 if sey < ssy:
                     sey, ssy = ssy, sey
 
                 self.select_start = ssx, ssy
                 self.select_end = sex, sey
 
-            if not event.state & Gdk.ModifierType.CONTROL_MASK:
-                if self.drag:
-                    self.drag = False
-                    self.undo_buff.add_state()
+            if self.drag:
+                self.drag = False
+                self.undo_buff.add_state()
 
         redr = False
 
         if self.velocity_editor:
             self.velocity_editor = None
             redr = True
 
@@ -1737,14 +1746,16 @@
             sey = self.edit[1]
 
         if self.select_start and self.select_end:
             ssx = min(self.select_start[0], len(self.trk) - 1)
             ssy = self.select_start[1]
             sex = min(self.select_end[0], len(self.trk) - 1)
             sey = self.select_end[1]
+        else:
+            return None
 
         # single row - don't copy if empty
         if ssy == sey:
             if self.trk[ssx][ssy].type == 0:
                 return None
 
         if sex < ssx:
```

### Comparing `vht-0.3.69/vht/trackviewpointer.py` & `vht-0.3.96/vht/trackviewpointer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht/velocityeditor.py` & `vht-0.3.96/vht/velocityeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.69/vht.egg-info/PKG-INFO` & `vht-0.3.96/vht.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.69
-Summary: vahatraker - a live MIDI sequencer for JACK
+Version: 0.3.96
+Summary: vahatraker - a live MIDI sequencer for pipewire/JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Intended Audience :: End Users/Desktop
@@ -28,15 +28,15 @@
 - live editing
 - fast workflow
 - intuitive midi-in
 - unheard of time signatures
 - scenes a'la 'ton
 - fractal turtles
 - fits on a floppy
-- doesn't make sound
+- doesn't make a sound
 
 Frankly speaking, vht was envisaged as a re-creation
 of seq24 in tracker form for author's "studio needs"
 and offers similar functionality (and limitations).
 It relies 100% on JACK audio connection kit for 
 input/output/synch and uses jack_capture for rendering.
 The GUI has similar dependencies as gnome-calculator
@@ -46,15 +46,13 @@
 Low level stuff was done in C and wrapped in Python.
 Human interfacing part of contraption employs
 GTK through gobject introspection and was also contrived
 in the language we shall no longer spam about.
 
 ## dependencies
 ```
-fedora - jack-audio-connection-kit-devel jack_capture
-ubuntu - libjack-jackd2-dev jack-capture
+pipewire-audio-client-libraries [jack_capture]
 ```
-
 ## install
 ```
 pip3 install vht
 ```
```

### Comparing `vht-0.3.69/vht.egg-info/SOURCES.txt` & `vht-0.3.96/vht.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-data/com.github.rdybka.vht.desktop
 data/mandy.png
 data/menu.ui
+data/net.sourceforge.projects.vht.desktop
+data/net.sourceforge.projects.vht.metainfo.xml
+data/net.sourceforge.projects.vht.svg
 data/vht.png
 data/vht.svg
 data/bank/10-gm1
 data/bank/20-gm2
 data/ctrl/10-gm
 data/ctrl/20-zyn
 doc/vht.1.gz
```

