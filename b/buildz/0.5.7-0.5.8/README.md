# Comparing `tmp/buildz-0.5.7.tar.gz` & `tmp/buildz-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.7.tar", last modified: Mon May 20 16:42:50 2024, max compression
+gzip compressed data, was "buildz-0.5.8.tar", last modified: Thu May 30 13:45:08 2024, max compression
```

## Comparing `buildz-0.5.7.tar` & `buildz-0.5.8.tar`

### file list

```diff
@@ -1,164 +1,166 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.193680 buildz-0.5.7/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.7/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2823 2024-05-20 16:42:50.193680 buildz-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.535085 buildz-0.5.7/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.7/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.7/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-05-07 11:40:11.000000 buildz-0.5.7/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.546087 buildz-0.5.7/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.553416 buildz-0.5.7/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.7/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.7/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.562518 buildz-0.5.7/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.7/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.7/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.562518 buildz-0.5.7/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.593651 buildz-0.5.7/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.7/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.7/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.7/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.7/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.7/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.625147 buildz-0.5.7/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.7/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.7/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.7/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.7/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.7/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-05-16 07:51:44.000000 buildz-0.5.7/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.635345 buildz-0.5.7/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.7/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.7/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.7/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.640932 buildz-0.5.7/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.7/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.7/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.650139 buildz-0.5.7/buildz/fz/
--rw-rw-rw-   0        0        0      285 2024-05-20 14:01:14.000000 buildz-0.5.7/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     2293 2024-05-20 08:56:56.000000 buildz-0.5.7/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      959 2024-05-20 09:16:37.000000 buildz-0.5.7/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     3425 2024-05-20 14:01:07.000000 buildz-0.5.7/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.656891 buildz-0.5.7/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.7/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      121 2024-05-16 11:49:03.000000 buildz-0.5.7/buildz/ioc/base.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.7/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.674153 buildz-0.5.7/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2554 2024-05-16 14:21:57.000000 buildz-0.5.7/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.7/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.7/buildz/ioc/ioc/confs.py
--rw-rw-rw-   0        0        0     1521 2024-05-16 15:35:31.000000 buildz-0.5.7/buildz/ioc/ioc/single.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.752259 buildz-0.5.7/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.7/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1255 2024-05-16 14:17:26.000000 buildz-0.5.7/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.942593 buildz-0.5.7/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/iocf_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.7/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0     1059 2024-05-16 14:13:56.000000 buildz-0.5.7/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      975 2024-05-16 14:13:36.000000 buildz-0.5.7/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.7/buildz/ioc/ioc_deal/iocf.py
--rw-rw-rw-   0        0        0      944 2024-05-16 14:13:13.000000 buildz-0.5.7/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1102 2024-05-16 14:12:34.000000 buildz-0.5.7/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1033 2024-05-16 14:17:05.000000 buildz-0.5.7/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6546 2024-05-16 15:31:49.000000 buildz-0.5.7/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1276 2024-05-16 14:15:31.000000 buildz-0.5.7/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      744 2024-05-16 14:45:17.000000 buildz-0.5.7/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.7/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     2295 2024-05-16 11:50:23.000000 buildz-0.5.7/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.944244 buildz-0.5.7/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.7/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.7/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.978280 buildz-0.5.7/buildz/xf/
--rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.7/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.7/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.7/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.006118 buildz-0.5.7/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.7/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.7/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.068699 buildz-0.5.7/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.7/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.7/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.7/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.7/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.7/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.7/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.7/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.7/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.7/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.7/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.7/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.7/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.7/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.7/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.099973 buildz-0.5.7/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.7/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.7/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.146745 buildz-0.5.7/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.7/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     2056 2024-05-16 07:51:17.000000 buildz-0.5.7/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1156 2024-05-16 07:57:06.000000 buildz-0.5.7/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.7/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.7/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.7/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.7/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.7/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.7/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3295 2024-05-14 07:15:35.000000 buildz-0.5.7/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.7/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.7/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.7/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.7/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.7/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.7/buildz/xf/loaderz/test1.py
--rw-rw-rw-   0        0        0     3379 2024-05-16 14:12:15.000000 buildz-0.5.7/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.7/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2746 2024-05-07 11:58:30.000000 buildz-0.5.7/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.7/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.7/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.162439 buildz-0.5.7/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.7/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.7/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.178068 buildz-0.5.7/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.7/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.7/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.7/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.7/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.7/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.7/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.7/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.7/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.535085 buildz-0.5.7/buildz.egg-info/
--rw-rw-rw-   0        0        0     2823 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3843 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 16:42:50.193680 buildz-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-05-20 16:41:30.000000 buildz-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.871557 buildz-0.5.8/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.8/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2823 2024-05-30 13:45:08.871557 buildz-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.379677 buildz-0.5.8/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.8/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.8/buildz/__main__.py
+-rw-rw-rw-   0        0        0     3530 2024-05-30 08:05:41.000000 buildz-0.5.8/buildz/argx.py
+-rw-rw-rw-   0        0        0     2324 2024-05-30 12:26:10.000000 buildz-0.5.8/buildz/cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.410089 buildz-0.5.8/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.425284 buildz-0.5.8/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.8/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.8/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.435724 buildz-0.5.8/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.8/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.8/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.450698 buildz-0.5.8/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.450698 buildz-0.5.8/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.8/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.8/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.8/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.8/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.8/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.457201 buildz-0.5.8/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.8/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.8/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.8/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.8/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.8/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-05-16 07:51:44.000000 buildz-0.5.8/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.457201 buildz-0.5.8/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.8/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.8/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.8/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.472902 buildz-0.5.8/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.8/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.8/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.472902 buildz-0.5.8/buildz/fz/
+-rw-rw-rw-   0        0        0      317 2024-05-30 13:16:11.000000 buildz-0.5.8/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     2293 2024-05-20 08:56:56.000000 buildz-0.5.8/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      285 2024-05-24 11:29:24.000000 buildz-0.5.8/buildz/fz/fhs.py
+-rw-rw-rw-   0        0        0     1298 2024-05-30 13:33:48.000000 buildz-0.5.8/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     3425 2024-05-20 14:01:07.000000 buildz-0.5.8/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.481262 buildz-0.5.8/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.8/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-05-16 11:49:03.000000 buildz-0.5.8/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.8/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.488768 buildz-0.5.8/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2554 2024-05-21 09:04:50.000000 buildz-0.5.8/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     7462 2024-05-22 09:13:57.000000 buildz-0.5.8/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13616 2024-05-30 06:10:36.000000 buildz-0.5.8/buildz/ioc/ioc/confs.py
+-rw-rw-rw-   0        0        0     1521 2024-05-16 15:35:31.000000 buildz-0.5.8/buildz/ioc/ioc/single.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.567910 buildz-0.5.8/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     6490 2024-05-21 12:22:23.000000 buildz-0.5.8/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1255 2024-05-16 14:17:26.000000 buildz-0.5.8/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.583950 buildz-0.5.8/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/iocf_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      352 2024-05-22 16:41:38.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.8/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.8/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0     1059 2024-05-16 14:13:56.000000 buildz-0.5.8/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      975 2024-05-16 14:13:36.000000 buildz-0.5.8/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.8/buildz/ioc/ioc_deal/iocf.py
+-rw-rw-rw-   0        0        0      944 2024-05-16 14:13:13.000000 buildz-0.5.8/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1102 2024-05-16 14:12:34.000000 buildz-0.5.8/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1033 2024-05-16 14:17:05.000000 buildz-0.5.8/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6546 2024-05-16 15:31:49.000000 buildz-0.5.8/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.8/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1276 2024-05-16 14:15:31.000000 buildz-0.5.8/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      744 2024-05-16 14:45:17.000000 buildz-0.5.8/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1023 2024-05-22 16:42:24.000000 buildz-0.5.8/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.8/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     2295 2024-05-16 11:50:23.000000 buildz-0.5.8/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.591737 buildz-0.5.8/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.8/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.8/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.631213 buildz-0.5.8/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.8/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.8/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.8/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.663028 buildz-0.5.8/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.8/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.8/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.710453 buildz-0.5.8/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.8/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.8/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.8/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.8/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.8/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.8/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.8/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.8/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.8/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.8/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.8/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.8/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.8/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.8/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.766606 buildz-0.5.8/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.8/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.8/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.806146 buildz-0.5.8/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      988 2024-05-29 06:52:25.000000 buildz-0.5.8/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     2056 2024-05-16 07:51:17.000000 buildz-0.5.8/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1156 2024-05-16 07:57:06.000000 buildz-0.5.8/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0     1168 2024-05-29 06:53:06.000000 buildz-0.5.8/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      775 2024-05-29 06:45:07.000000 buildz-0.5.8/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.8/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.8/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      429 2024-05-29 06:44:45.000000 buildz-0.5.8/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.8/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     5683 2024-05-29 06:49:29.000000 buildz-0.5.8/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.8/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.8/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.8/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.8/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.8/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0      110 2024-05-29 06:55:41.000000 buildz-0.5.8/buildz/xf/loaderz/test1.py
+-rw-rw-rw-   0        0        0     3681 2024-05-22 10:11:30.000000 buildz-0.5.8/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.8/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2815 2024-05-29 06:56:33.000000 buildz-0.5.8/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.8/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.8/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.821792 buildz-0.5.8/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.8/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.8/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.870563 buildz-0.5.8/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.8/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.8/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.8/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.8/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.8/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.8/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.8/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.8/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-05-30 13:45:08.393801 buildz-0.5.8/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2823 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3874 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 13:45:08.000000 buildz-0.5.8/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 13:45:08.871557 buildz-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-05-30 13:42:20.000000 buildz-0.5.8/setup.py
```

### Comparing `buildz-0.5.7/LICENSE` & `buildz-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/PKG-INFO` & `buildz-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.7
+Version: 0.5.8
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.7/README.md` & `buildz-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/argx.py` & `buildz-0.5.8/buildz/argx.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,32 @@
 
     但更简单的方法是:
     xf.args("{id:'001', name: zero, kind: life, age: 12}".split(" ")) = {'id': '001', 'name': 'zero', 'kind': 'life', 'age': 12}
     python buildz.xf {id:'001', name: zero, kind: life, age: 12}
     就是对引号不太适用
     """
     def __init__(self, args = [], maps ={}):
+        args = [maps[k] if k in maps else k for k in args]
         self.args = args
         self.maps = maps
+    def des(self):
+        cmd = " ".join(self.args)
+        adds = []
+        for k, val in self.maps.items():
+            tmp = f"    [-{k} param] [--{val}=param]"
+            adds.append(tmp)
+        adds = [cmd]+adds
+        rs = "\n".join(adds)
+        return rs
+    def check(self, args, ks):
+        rst = []
+        for k in ks:
+            if k not in args:
+                rst.append(k)
+        return rst
     def __call__(self, argv = None):
         args, maps = fetch(argv)
         rst = {}
         for i in range(len(args)):
             if i >= len(self.args):
                 break
             key = self.args[i]
@@ -32,14 +48,19 @@
             if key in rst:
                 val = rst[key]
                 rst[rkey] = val
                 del rst[key]
         return rst
 
 pass
+class FetchX(Fetch):
+    def __init__(self, *a, **b):
+        super().__init__(a,b)
+
+pass
 def fetch(argv = None):
     r"""
     format: a b c -a 123 -b456 --c=789 +d  -x"??? ???" y z
     return: [a,b,c,y,z], {a:123,b:456,c:789,d:1,x:'??? ???'}
     """
     if argv is None:
         argv = sys.argv[1:]
```

### Comparing `buildz-0.5.7/buildz/demo/ioc/deal.py` & `buildz-0.5.8/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/ioc/help.py` & `buildz-0.5.8/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/myers/deal.py` & `buildz-0.5.8/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/res/conf/main.js` & `buildz-0.5.8/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/res/help/ioc.js` & `buildz-0.5.8/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/res/help/myers.js` & `buildz-0.5.8/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/res/help/search.js` & `buildz-0.5.8/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/res/help/xf.js` & `buildz-0.5.8/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/res/test.js` & `buildz-0.5.8/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/search/deal.py` & `buildz-0.5.8/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/demo/test.py` & `buildz-0.5.8/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/fz/dirz.py` & `buildz-0.5.8/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/fz/lsf.py` & `buildz-0.5.8/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc/base.py` & `buildz-0.5.8/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc/conf.py` & `buildz-0.5.8/buildz/ioc/ioc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,16 +129,27 @@
         if self.confs.global_deal and search_confs:
             return self.confs.get_deal(type, self.id)
         if type in self.deals:
             return self.deals[type]
         if not search_confs:
             return None
         return self.confs.get_deal(type, self.id)
+    def get_data_conf(self, data, src = None, info = None):
+        if type(data) not in [list, dict, tuple]:
+            i = self.confs.data_index_type[0]
+            data = [self.default_type(), data]
+            if i != 0:
+                data.reverse()
+        _type = self.confs.get_data_type(data, 1, self.default_type())
+        edata = EncapeData(data, self, local=True, type=_type, src = src, info = info)
+        return edata
     def get_data(self, id, local = True, search_confs = True, src = None, info = None):
         self.do_init()
+        if type(id) in [list, tuple, dict]:
+            return self.get_data_conf(id, src, info)
         if id in self.datas:
             obj = self.datas[id]
             edata = EncapeData(obj, self, local = False, src=src, info = info)
             if _id(obj) != _id(edata.data):
                 # 有parent，做了填充，用填充后的替换
                 self.datas[id] = edata.data
             return edata
```

### Comparing `buildz-0.5.7/buildz/ioc/ioc/confs.py` & `buildz-0.5.8/buildz/ioc/ioc/confs.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,19 @@
             例: ids = ['a','b','c'], spt = ".", id = 'a.b.c', 
         """
         return self.spt.join(ids)
     def add_fps(self, fps):
         for fp in fps:
             self.add_fp(fp)
     def add_fp(self, fp):
-        conf = self.loads(xf.fread(fp))
+        try:
+            conf = self.loads(xf.fread(fp))
+        except:
+            print(f'error in loads: {fp}')
+            raise
         return self.add(conf)
     def adds(self, confs):
         for conf in confs:
             self.add(conf)
     def add(self, conf):
         """
             {
```

### Comparing `buildz-0.5.7/buildz/ioc/ioc/single.py` & `buildz-0.5.8/buildz/ioc/ioc/single.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -119,15 +119,26 @@
 
 class BaseDeal(Base):
     """
         基础处理类，加了一些方便处理的方法，自己写的处理可以不用继承这个
         自己实现的处理类，要实现两个方法：__call__(self, edata:EncapeData)和remove(self, edata:EncapeData)
         其中remove可以只写个空方法
     """
+    def get_data(self, data, conf, src = None, info = None):
+        if type(data) not in [list, dict, tuple]:
+            i = conf.confs.data_index_type[0]
+            data = [conf.default_type(), data]
+            if i != 0:
+                data.reverse()
+        _type = conf.confs.get_data_type(data, 1, conf.default_type())
+        edata = EncapeData(data, conf, local=True, type=_type, src = src, info = info)
+        return edata
     def get_obj(self, data, conf, src = None, info = None):
+        edata = self.get_data(data, conf, src, info)
+        return edata()
         if type(data) not in [list, dict, tuple]:
             i = conf.confs.data_index_type[0]
             data = [conf.default_type(), data]
             if i != 0:
                 data.reverse()
         _type = conf.confs.get_data_type(data, 1, conf.default_type())
         edata = EncapeData(data, conf, local=True, type=_type, src = src, info = info)
```

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.8/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.8/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/conf/ref_lists.js` & `buildz-0.5.8/buildz/ioc/ioc_deal/conf/ref_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/iocf.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/iocf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/var.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 join = os.path.join
 class VarDeal(FormatDeal):
     """
         代码变量var:
             {
                 id:id
                 type: var
-                key: string
+                data: string
             }
         简写:
-            [[id, var], key]
-            [var, key]
+            [[id, var], data]
+            [var, data]
         例:
             [var, buildz.pyz.is_windows] // 返回buildz.pyz下的is_windows
     """
     def init(self, fp_lists = None, fp_defaults = None):
         self.singles = {}
         self.sources = {}
         super().init("VarDeal", fp_lists, fp_defaults, 
             join(dp, "conf", "var_lists.js"))
     def deal(self, edata:EncapeData):
         sid = edata.sid
         data = edata.data
         conf = edata.conf
         data = self.format(data)
         src = edata.src
-        key = xf.g(data, key=0)
+        key = xf.get_first(data, "var", "data")
         key = pyz.load(key)
         return key
 
 pass
```

### Comparing `buildz-0.5.7/buildz/ioc/ioc_deal/xfile.py` & `buildz-0.5.8/buildz/ioc/ioc_deal/xfile.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/pyz.py` & `buildz-0.5.8/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/tz/myers_diff.py` & `buildz-0.5.8/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/file.py` & `buildz-0.5.8/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/base.py` & `buildz-0.5.8/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/buffer.py` & `buildz-0.5.8/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/listz.py` & `buildz-0.5.8/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/lr.py` & `buildz-0.5.8/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.8/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.8/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.8/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/reval.py` & `buildz-0.5.8/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/setz.py` & `buildz-0.5.8/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/spt.py` & `buildz-0.5.8/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/deal/strz.py` & `buildz-0.5.8/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/item.py` & `buildz-0.5.8/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/mg.py` & `buildz-0.5.8/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loader/pos.py` & `buildz-0.5.8/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/base.py` & `buildz-0.5.8/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/buffer.py` & `buildz-0.5.8/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/listz.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     def init(self, left, right):
         super().init(left, right, 'list')
     def types(self):
         return ['']
     def build(self, obj):
         val = obj.val
         if type(val)!=list:
+            return None
             obj.is_val = 1
             return obj
         if len(val)==0:
             obj.val = ''
             obj.is_val = 1
             return obj
         if len(val)>1:
```

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/mapz.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     def init(self, left, right):
         super().init(left, right, "map")
     def types(self):
         return ['']
     def build(self, obj):
         val = obj.val
         if type(val)!=list:
+            return None
             obj.is_val = 1
             return obj
         if len(val)==0:
             obj.val = ''
             obj.is_val = 1
             return obj
         if len(val)%3!=0:
```

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/nextz.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/nextz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from .. import base
 from .. import item
 
 class PrevNextDeal(base.BaseDeal):
     def labels(self):
         return ['']
-    def types(self):
-        return [""]
+    #def types(self):
+    #    return [""]
     """
         读取下一个字符放缓存里，应放最低优先级
     """
     def deal(self, buffer, arr, mg):
         c = buffer.read_cache(1)
         if len(c)==0:
             rm = buffer.full().strip()
             buffer.clean()
             if len(rm)==0:
                 return False
             obj = item.Item(rm, type = '', is_val = 0)
             arr.append(obj)
+            # TODO return True?
             return False
         return True
     def build(self, obj):
         if type(obj.val)==list:
             return None
         obj.is_val = 1
         return obj
```

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.8/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/item.py` & `buildz-0.5.8/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/mg.py` & `buildz-0.5.8/buildz/xf/loaderz/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/pos.py` & `buildz-0.5.8/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/loaderz/test.py` & `buildz-0.5.8/buildz/xf/loaderz/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/mapz.py` & `buildz-0.5.8/buildz/xf/mapz.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,109 +104,128 @@
 00000670: 2072 6574 7572 6e20 7273 740d 0a0d 0a70   return rst....p
 00000680: 6173 730d 0a64 6566 2073 286f 626a 2c20  ass..def s(obj, 
 00000690: 2a2a 6d61 7073 293a 0d0a 2020 2020 666f  **maps):..    fo
 000006a0: 7220 6b20 696e 206d 6170 733a 0d0a 2020  r k in maps:..  
 000006b0: 2020 2020 2020 7620 3d20 6d61 7073 5b6b        v = maps[k
 000006c0: 5d0d 0a20 2020 2020 2020 206f 626a 5b6b  ]..        obj[k
 000006d0: 5d20 3d20 760d 0a0d 0a70 6173 730d 0a64  ] = v....pass..d
-000006e0: 6566 2073 6574 7328 6d61 7073 2c20 6b65  ef sets(maps, ke
-000006f0: 7973 2c20 7661 6c29 3a0d 0a20 2020 2069  ys, val):..    i
-00000700: 6620 7479 7065 286b 6579 7329 2021 3d20  f type(keys) != 
-00000710: 6c69 7374 3a0d 0a20 2020 2020 2020 206b  list:..        k
-00000720: 6579 7320 3d20 5b6b 6579 735d 0d0a 2020  eys = [keys]..  
-00000730: 2020 666f 7220 6b65 7920 696e 206b 6579    for key in key
-00000740: 735b 3a2d 315d 3a0d 0a20 2020 2020 2020  s[:-1]:..       
-00000750: 2069 6620 6b65 7920 6e6f 7420 696e 206d   if key not in m
-00000760: 6170 733a 0d0a 2020 2020 2020 2020 2020  aps:..          
-00000770: 2020 6d61 7073 5b6b 6579 5d20 3d20 7b7d    maps[key] = {}
-00000780: 0d0a 2020 2020 2020 2020 6d61 7073 203d  ..        maps =
-00000790: 206d 6170 735b 6b65 795d 0d0a 2020 2020   maps[key]..    
-000007a0: 6d61 7073 5b6b 6579 735b 2d31 5d5d 203d  maps[keys[-1]] =
-000007b0: 2076 616c 0d0a 0d0a 7061 7373 0d0a 6465   val....pass..de
-000007c0: 6620 6765 7473 286d 6170 732c 206b 6579  f gets(maps, key
-000007d0: 732c 2064 6566 6175 6c74 203d 204e 6f6e  s, default = Non
-000007e0: 6529 3a0d 0a20 2020 2069 6620 7479 7065  e):..    if type
-000007f0: 286b 6579 7329 2021 3d20 6c69 7374 3a0d  (keys) != list:.
-00000800: 0a20 2020 2020 2020 206b 6579 7320 3d20  .        keys = 
-00000810: 5b6b 6579 735d 0d0a 2020 2020 666f 7220  [keys]..    for 
-00000820: 6b65 7920 696e 206b 6579 733a 0d0a 2020  key in keys:..  
-00000830: 2020 2020 2020 6966 206b 6579 206e 6f74        if key not
-00000840: 2069 6e20 6d61 7073 3a0d 0a20 2020 2020   in maps:..     
-00000850: 2020 2020 2020 2072 6574 7572 6e20 6465         return de
-00000860: 6661 756c 740d 0a20 2020 2020 2020 206d  fault..        m
-00000870: 6170 7320 3d20 6d61 7073 5b6b 6579 5d0d  aps = maps[key].
-00000880: 0a20 2020 2072 6574 7572 6e20 6d61 7073  .    return maps
-00000890: 0d0a 0d0a 7061 7373 0d0a 6465 6620 7265  ....pass..def re
-000008a0: 6d6f 7665 7328 6d61 7073 2c20 6b65 7973  moves(maps, keys
-000008b0: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
-000008c0: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
-000008d0: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
-000008e0: 6b65 7973 5d0d 0a20 2020 2061 7272 203d  keys]..    arr =
-000008f0: 205b 5d0d 0a20 2020 2066 6f72 206b 6579   []..    for key
-00000900: 2069 6e20 6b65 7973 3a0d 0a20 2020 2020   in keys:..     
-00000910: 2020 2069 6620 6b65 7920 6e6f 7420 696e     if key not in
-00000920: 206d 6170 733a 0d0a 2020 2020 2020 2020   maps:..        
-00000930: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-00000940: 2020 2061 7272 2e61 7070 656e 6428 5b6d     arr.append([m
-00000950: 6170 732c 206b 6579 5d29 0d0a 2020 2020  aps, key])..    
-00000960: 2020 2020 6d61 7073 203d 206d 6170 735b      maps = maps[
-00000970: 6b65 795d 0d0a 2020 2020 6172 722e 7265  key]..    arr.re
-00000980: 7665 7273 6528 290d 0a20 2020 2066 6972  verse()..    fir
-00000990: 7374 3d31 0d0a 2020 2020 666f 7220 6d61  st=1..    for ma
-000009a0: 7073 2c6b 6579 2069 6e20 6172 723a 0d0a  ps,key in arr:..
-000009b0: 2020 2020 2020 2020 6966 2066 6972 7374          if first
-000009c0: 206f 7220 6c65 6e28 6d61 7073 5b6b 6579   or len(maps[key
-000009d0: 5d29 3d3d 303a 0d0a 2020 2020 2020 2020  ])==0:..        
-000009e0: 2020 2020 6465 6c20 6d61 7073 5b6b 6579      del maps[key
-000009f0: 5d0d 0a20 2020 2020 2020 2066 6972 7374  ]..        first
-00000a00: 3d30 0d0a 2020 2020 7265 7475 726e 204e  =0..    return N
-00000a10: 6f6e 650d 0a0d 0a70 6173 730d 0a64 6566  one....pass..def
-00000a20: 206c 326d 2861 7272 2c20 2a2a 6d61 7073   l2m(arr, **maps
-00000a30: 293a 0d0a 2020 2020 7273 7420 3d20 7b7d  ):..    rst = {}
-00000a40: 0d0a 2020 2020 6920 3d20 300d 0a20 2020  ..    i = 0..   
-00000a50: 2066 6f72 206b 2069 6e20 6d61 7073 3a0d   for k in maps:.
-00000a60: 0a20 2020 2020 2020 2069 6620 693c 6c65  .        if i<le
-00000a70: 6e28 6172 7229 3a0d 0a20 2020 2020 2020  n(arr):..       
-00000a80: 2020 2020 2076 616c 203d 2061 7272 5b69       val = arr[i
-00000a90: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
-00000aa0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-00000ab0: 6c20 3d20 6d61 7073 5b6b 5d0d 0a20 2020  l = maps[k]..   
-00000ac0: 2020 2020 2072 7374 5b6b 5d20 3d20 7661       rst[k] = va
-00000ad0: 6c0d 0a20 2020 2020 2020 2069 2b3d 310d  l..        i+=1.
-00000ae0: 0a20 2020 2072 6574 7572 6e20 7273 740d  .    return rst.
-00000af0: 0a0d 0a70 6173 730d 0a0d 0a64 6566 2064  ...pass....def d
-00000b00: 6565 705f 7570 6461 7465 2874 6172 6765  eep_update(targe
-00000b10: 742c 2073 7263 2c20 7265 706c 6163 653d  t, src, replace=
-00000b20: 3129 3a0d 0a20 2020 2022 2222 0d0a 2020  1):..    """..  
-00000b30: 2020 2020 2020 6469 6374 e6b7 b1e5 b182        dict......
-00000b40: e69b b4e6 96b0 efbc 8c73 7263 5b6b 6579  .........src[key
-00000b50: 5de6 98af 6469 6374 e5b0 b1e6 b7b1 e585  ]...dict........
-00000b60: a5e6 9bb4 e696 b0ef bc8c e590 a6e5 8899  ................
-00000b70: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00000b80: 7263 e69c 89e8 808c 7461 7267 6574 e6b2  rc......target..
-00000b90: a1e6 9c89 e5b0 b1e6 9bbf e68d a2ef bc8c  ................
-00000ba0: e590 a6e5 8899 efbc 9a0d 0a20 2020 2020  ...........     
-00000bb0: 2020 2020 2020 2020 2020 2072 6570 6c61             repla
-00000bc0: 6365 3d31 e5b0 b1e6 9bbf e68d a20d 0a20  ce=1........... 
-00000bd0: 2020 2022 2222 0d0a 2020 2020 666f 7220     """..    for 
-00000be0: 6b20 696e 2073 7263 3a0d 0a20 2020 2020  k in src:..     
-00000bf0: 2020 2076 616c 203d 2073 7263 5b6b 5d0d     val = src[k].
-00000c00: 0a20 2020 2020 2020 2069 6620 6b20 6e6f  .        if k no
-00000c10: 7420 696e 2074 6172 6765 743a 0d0a 2020  t in target:..  
-00000c20: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00000c30: 5b6b 5d20 3d20 7661 6c0d 0a20 2020 2020  [k] = val..     
-00000c40: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00000c50: 0a20 2020 2020 2020 206d 7661 6c20 3d20  .        mval = 
-00000c60: 7461 7267 6574 5b6b 5d0d 0a20 2020 2020  target[k]..     
-00000c70: 2020 2069 6620 7479 7065 286d 7661 6c29     if type(mval)
-00000c80: 203d 3d20 6469 6374 2061 6e64 2074 7970   == dict and typ
-00000c90: 6528 7661 6c29 3d3d 6469 6374 3a0d 0a20  e(val)==dict:.. 
-00000ca0: 2020 2020 2020 2020 2020 2064 6565 705f             deep_
-00000cb0: 7570 6461 7465 286d 7661 6c2c 2076 616c  update(mval, val
-00000cc0: 2c20 7265 706c 6163 6529 0d0a 2020 2020  , replace)..    
-00000cd0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000ce0: 2020 2020 2020 2069 6620 7265 706c 6163         if replac
-00000cf0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000d00: 2020 2020 7461 7267 6574 5b6b 5d20 3d20      target[k] = 
-00000d10: 7661 6c0d 0a0d 0a70 6173 730d 0a75 7064  val....pass..upd
-00000d20: 6174 6520 3d20 6465 6570 5f75 7064 6174  ate = deep_updat
-00000d30: 650d 0a                                  e..
+000006e0: 6566 2066 696c 6c5f 6663 286d 6170 732c  ef fill_fc(maps,
+000006f0: 2066 6329 3a0d 0a20 2020 2066 6f72 206b   fc):..    for k
+00000700: 2069 6e20 6d61 7073 3a0d 0a20 2020 2020   in maps:..     
+00000710: 2020 2076 203d 206d 6170 735b 6b5d 0d0a     v = maps[k]..
+00000720: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
+00000730: 7629 203d 3d20 6469 6374 3a0d 0a20 2020  v) == dict:..   
+00000740: 2020 2020 2020 2020 2066 696c 6c5f 6663           fill_fc
+00000750: 2876 2c20 6663 290d 0a20 2020 2020 2020  (v, fc)..       
+00000760: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00000770: 2020 2020 2020 206d 6170 735b 6b5d 203d         maps[k] =
+00000780: 2066 6328 7629 0d0a 2020 2020 7265 7475   fc(v)..    retu
+00000790: 726e 206d 6170 730d 0a0d 0a70 6173 730d  rn maps....pass.
+000007a0: 0a64 6566 2073 6574 7328 6d61 7073 2c20  .def sets(maps, 
+000007b0: 6b65 7973 2c20 7661 6c29 3a0d 0a20 2020  keys, val):..   
+000007c0: 2069 6620 7479 7065 286b 6579 7329 2021   if type(keys) !
+000007d0: 3d20 6c69 7374 3a0d 0a20 2020 2020 2020  = list:..       
+000007e0: 206b 6579 7320 3d20 5b6b 6579 735d 0d0a   keys = [keys]..
+000007f0: 2020 2020 666f 7220 6b65 7920 696e 206b      for key in k
+00000800: 6579 735b 3a2d 315d 3a0d 0a20 2020 2020  eys[:-1]:..     
+00000810: 2020 2069 6620 6b65 7920 6e6f 7420 696e     if key not in
+00000820: 206d 6170 733a 0d0a 2020 2020 2020 2020   maps:..        
+00000830: 2020 2020 6d61 7073 5b6b 6579 5d20 3d20      maps[key] = 
+00000840: 7b7d 0d0a 2020 2020 2020 2020 6d61 7073  {}..        maps
+00000850: 203d 206d 6170 735b 6b65 795d 0d0a 2020   = maps[key]..  
+00000860: 2020 6d61 7073 5b6b 6579 735b 2d31 5d5d    maps[keys[-1]]
+00000870: 203d 2076 616c 0d0a 0d0a 7061 7373 0d0a   = val....pass..
+00000880: 6465 6620 6765 7473 286d 6170 732c 206b  def gets(maps, k
+00000890: 6579 732c 2064 6566 6175 6c74 203d 204e  eys, default = N
+000008a0: 6f6e 6529 3a0d 0a20 2020 2069 6620 7479  one):..    if ty
+000008b0: 7065 286b 6579 7329 2021 3d20 6c69 7374  pe(keys) != list
+000008c0: 3a0d 0a20 2020 2020 2020 206b 6579 7320  :..        keys 
+000008d0: 3d20 5b6b 6579 735d 0d0a 2020 2020 666f  = [keys]..    fo
+000008e0: 7220 6b65 7920 696e 206b 6579 733a 0d0a  r key in keys:..
+000008f0: 2020 2020 2020 2020 6966 206b 6579 206e          if key n
+00000900: 6f74 2069 6e20 6d61 7073 3a0d 0a20 2020  ot in maps:..   
+00000910: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000920: 6465 6661 756c 740d 0a20 2020 2020 2020  default..       
+00000930: 206d 6170 7320 3d20 6d61 7073 5b6b 6579   maps = maps[key
+00000940: 5d0d 0a20 2020 2072 6574 7572 6e20 6d61  ]..    return ma
+00000950: 7073 0d0a 0d0a 7061 7373 0d0a 6465 6620  ps....pass..def 
+00000960: 7265 6d6f 7665 7328 6d61 7073 2c20 6b65  removes(maps, ke
+00000970: 7973 293a 0d0a 2020 2020 6966 2074 7970  ys):..    if typ
+00000980: 6528 6b65 7973 2920 213d 206c 6973 743a  e(keys) != list:
+00000990: 0d0a 2020 2020 2020 2020 6b65 7973 203d  ..        keys =
+000009a0: 205b 6b65 7973 5d0d 0a20 2020 2061 7272   [keys]..    arr
+000009b0: 203d 205b 5d0d 0a20 2020 2066 6f72 206b   = []..    for k
+000009c0: 6579 2069 6e20 6b65 7973 3a0d 0a20 2020  ey in keys:..   
+000009d0: 2020 2020 2069 6620 6b65 7920 6e6f 7420       if key not 
+000009e0: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
+000009f0: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
+00000a00: 2020 2020 2061 7272 2e61 7070 656e 6428       arr.append(
+00000a10: 5b6d 6170 732c 206b 6579 5d29 0d0a 2020  [maps, key])..  
+00000a20: 2020 2020 2020 6d61 7073 203d 206d 6170        maps = map
+00000a30: 735b 6b65 795d 0d0a 2020 2020 6172 722e  s[key]..    arr.
+00000a40: 7265 7665 7273 6528 290d 0a20 2020 2066  reverse()..    f
+00000a50: 6972 7374 3d31 0d0a 2020 2020 666f 7220  irst=1..    for 
+00000a60: 6d61 7073 2c6b 6579 2069 6e20 6172 723a  maps,key in arr:
+00000a70: 0d0a 2020 2020 2020 2020 6966 2066 6972  ..        if fir
+00000a80: 7374 206f 7220 6c65 6e28 6d61 7073 5b6b  st or len(maps[k
+00000a90: 6579 5d29 3d3d 303a 0d0a 2020 2020 2020  ey])==0:..      
+00000aa0: 2020 2020 2020 6465 6c20 6d61 7073 5b6b        del maps[k
+00000ab0: 6579 5d0d 0a20 2020 2020 2020 2066 6972  ey]..        fir
+00000ac0: 7374 3d30 0d0a 2020 2020 7265 7475 726e  st=0..    return
+00000ad0: 204e 6f6e 650d 0a0d 0a70 6173 730d 0a64   None....pass..d
+00000ae0: 6566 206c 326d 2861 7272 2c20 2a2a 6d61  ef l2m(arr, **ma
+00000af0: 7073 293a 0d0a 2020 2020 7273 7420 3d20  ps):..    rst = 
+00000b00: 7b7d 0d0a 2020 2020 6920 3d20 300d 0a20  {}..    i = 0.. 
+00000b10: 2020 2066 6f72 206b 2069 6e20 6d61 7073     for k in maps
+00000b20: 3a0d 0a20 2020 2020 2020 2069 6620 693c  :..        if i<
+00000b30: 6c65 6e28 6172 7229 3a0d 0a20 2020 2020  len(arr):..     
+00000b40: 2020 2020 2020 2076 616c 203d 2061 7272         val = arr
+00000b50: 5b69 5d0d 0a20 2020 2020 2020 2065 6c73  [i]..        els
+00000b60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000b70: 7661 6c20 3d20 6d61 7073 5b6b 5d0d 0a20  val = maps[k].. 
+00000b80: 2020 2020 2020 2072 7374 5b6b 5d20 3d20         rst[k] = 
+00000b90: 7661 6c0d 0a20 2020 2020 2020 2069 2b3d  val..        i+=
+00000ba0: 310d 0a20 2020 2072 6574 7572 6e20 7273  1..    return rs
+00000bb0: 740d 0a0d 0a70 6173 730d 0a0d 0a64 6566  t....pass....def
+00000bc0: 2064 6565 705f 7570 6461 7465 2874 6172   deep_update(tar
+00000bd0: 6765 742c 2073 7263 2c20 7265 706c 6163  get, src, replac
+00000be0: 653d 3129 3a0d 0a20 2020 2022 2222 0d0a  e=1):..    """..
+00000bf0: 2020 2020 2020 2020 6469 6374 e6b7 b1e5          dict....
+00000c00: b182 e69b b4e6 96b0 efbc 8c73 7263 5b6b  ...........src[k
+00000c10: 6579 5de6 98af 6469 6374 e5b0 b1e6 b7b1  ey]...dict......
+00000c20: e585 a5e6 9bb4 e696 b0ef bc8c e590 a6e5  ................
+00000c30: 8899 3a0d 0a20 2020 2020 2020 2020 2020  ..:..           
+00000c40: 2073 7263 e69c 89e8 808c 7461 7267 6574   src......target
+00000c50: e6b2 a1e6 9c89 e5b0 b1e6 9bbf e68d a2ef  ................
+00000c60: bc8c e590 a6e5 8899 efbc 9a0d 0a20 2020  .............   
+00000c70: 2020 2020 2020 2020 2020 2020 2072 6570               rep
+00000c80: 6c61 6365 3d31 e5b0 b1e6 9bbf e68d a20d  lace=1..........
+00000c90: 0a20 2020 2022 2222 0d0a 2020 2020 666f  .    """..    fo
+00000ca0: 7220 6b20 696e 2073 7263 3a0d 0a20 2020  r k in src:..   
+00000cb0: 2020 2020 2076 616c 203d 2073 7263 5b6b       val = src[k
+00000cc0: 5d0d 0a20 2020 2020 2020 2069 6620 6b20  ]..        if k 
+00000cd0: 6e6f 7420 696e 2074 6172 6765 743a 0d0a  not in target:..
+00000ce0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+00000cf0: 6574 5b6b 5d20 3d20 7661 6c0d 0a20 2020  et[k] = val..   
+00000d00: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00000d10: 650d 0a20 2020 2020 2020 206d 7661 6c20  e..        mval 
+00000d20: 3d20 7461 7267 6574 5b6b 5d0d 0a20 2020  = target[k]..   
+00000d30: 2020 2020 2069 6620 7479 7065 286d 7661       if type(mva
+00000d40: 6c29 203d 3d20 6469 6374 2061 6e64 2074  l) == dict and t
+00000d50: 7970 6528 7661 6c29 3d3d 6469 6374 3a0d  ype(val)==dict:.
+00000d60: 0a20 2020 2020 2020 2020 2020 2064 6565  .            dee
+00000d70: 705f 7570 6461 7465 286d 7661 6c2c 2076  p_update(mval, v
+00000d80: 616c 2c20 7265 706c 6163 6529 0d0a 2020  al, replace)..  
+00000d90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00000da0: 2020 2020 2020 2020 2069 6620 7265 706c           if repl
+00000db0: 6163 653a 0d0a 2020 2020 2020 2020 2020  ace:..          
+00000dc0: 2020 2020 2020 7461 7267 6574 5b6b 5d20        target[k] 
+00000dd0: 3d20 7661 6c0d 0a0d 0a70 6173 730d 0a75  = val....pass..u
+00000de0: 7064 6174 6520 3d20 6465 6570 5f75 7064  pdate = deep_upd
+00000df0: 6174 650d 0a64 6566 2064 6565 705f 6669  ate..def deep_fi
+00000e00: 6c6c 2873 7263 2c20 7461 7267 6574 2c20  ll(src, target, 
+00000e10: 7265 706c 6163 653d 3129 3a0d 0a20 2020  replace=1):..   
+00000e20: 2072 6574 7572 6e20 6465 6570 5f75 7064   return deep_upd
+00000e30: 6174 6528 7461 7267 6574 2c20 7372 632c  ate(target, src,
+00000e40: 2072 6570 6c61 6365 290d 0a0d 0a70 6173   replace)....pas
+00000e50: 730d 0a66 696c 6c3d 6465 6570 5f66 696c  s..fill=deep_fil
+00000e60: 6c                                       l
```

### Comparing `buildz-0.5.7/buildz/xf/read.py` & `buildz-0.5.8/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/readz.py` & `buildz-0.5.8/buildz/xf/readz.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,19 @@
     mgs.add(reval.ValDeal("true", lambda x:True))
     mgs.add(reval.ValDeal("false", lambda x:False))
 
 pass
 def build(as_bytes=False):
     mgs = mg.Manager(as_bytes)
     build_val(mgs)
+    #1,0,0,1: 没引号当r"..."
+    #1,0,1,1: 没引导当"..."
     mgs.add(strz.PrevStrDeal("r'''","'''",0,0,0))
     mgs.add(strz.PrevStrDeal('r"""','"""',0,0,0))
-    mgs.add(strz.PrevStrDeal("r'","'",1,0,0))
+    mgs.add(strz.PrevStrDeal("r'","'",1,0,0,1))
     mgs.add(strz.PrevStrDeal('r"','"',1,0,0))
     mgs.add(strz.PrevStrDeal("###","###",0,1))
     mgs.add(strz.PrevStrDeal("/*","*/",0,1))
     mgs.add(strz.PrevStrDeal("'''","'''",0,0,1))
     mgs.add(strz.PrevStrDeal('"""','"""',0,0,1))
     mgs.add(strz.PrevStrDeal("#","\n",1,1))
     mgs.add(strz.PrevStrDeal("//","\n",1,1))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildz-0.5.7/buildz/xf/stack.py` & `buildz-0.5.8/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/write.py` & `buildz-0.5.8/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/base.py` & `buildz-0.5.8/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/conf.py` & `buildz-0.5.8/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/deal/listz.py` & `buildz-0.5.8/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.8/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/deal/strz.py` & `buildz-0.5.8/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/itemz.py` & `buildz-0.5.8/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/writer/mg.py` & `buildz-0.5.8/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz/xf/xargs.py` & `buildz-0.5.8/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.7/buildz.egg-info/PKG-INFO` & `buildz-0.5.8/buildz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.7
+Version: 0.5.8
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.7/buildz.egg-info/SOURCES.txt` & `buildz-0.5.8/buildz.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 buildz/__init__.py
 buildz/__main__.py
 buildz/argx.py
+buildz/cmd.py
 buildz/pyz.py
 buildz.egg-info/PKG-INFO
 buildz.egg-info/SOURCES.txt
 buildz.egg-info/dependency_links.txt
 buildz.egg-info/top_level.txt
 buildz/demo/test.py
 buildz/demo/ioc/deal.py
@@ -28,14 +29,15 @@
 buildz/demo/res/help/xf.js
 buildz/demo/search/deal.py
 buildz/demo/search/help.py
 buildz/demo/xf/deal.py
 buildz/demo/xf/help.py
 buildz/fz/__init__.py
 buildz/fz/dirz.py
+buildz/fz/fhs.py
 buildz/fz/fio.py
 buildz/fz/lsf.py
 buildz/ioc/__init__.py
 buildz/ioc/base.py
 buildz/ioc/init.py
 buildz/ioc/ioc/base.py
 buildz/ioc/ioc/conf.py
```

### Comparing `buildz-0.5.7/setup.py` & `buildz-0.5.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.7',
+    version = '0.5.8',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

