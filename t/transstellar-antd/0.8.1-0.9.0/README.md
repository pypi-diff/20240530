# Comparing `tmp/transstellar_antd-0.8.1.tar.gz` & `tmp/transstellar_antd-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transstellar_antd-0.8.1.tar", max compression
+gzip compressed data, was "transstellar_antd-0.9.0.tar", max compression
```

## Comparing `transstellar_antd-0.8.1.tar` & `transstellar_antd-0.9.0.tar`

### file list

```diff
@@ -1,161 +1,167 @@
--rw-r--r--   0        0        0      388 2024-05-21 06:50:54.306719 transstellar_antd-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      923 2024-05-21 02:37:34.091601 transstellar_antd-0.8.1/src/transstellar_antd/__init__.py
--rw-r--r--   0        0        0      727 2024-05-21 02:42:18.474373 transstellar_antd-0.8.1/src/transstellar_antd/components/__init__.py
--rw-r--r--   0        0        0      922 2024-05-21 02:44:50.391485 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      267 2024-02-27 04:17:55.380208 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      810 2024-03-27 08:44:31.501813 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/anchor.cpython-312.pyc
--rw-r--r--   0        0        0      454 2024-05-21 02:39:34.444908 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/breadcrumb.cpython-312.pyc
--rw-r--r--   0        0        0      844 2024-03-25 09:53:39.649429 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/button.cpython-312.pyc
--rw-r--r--   0        0        0      795 2024-03-06 06:52:35.091364 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0     1868 2024-05-14 09:46:23.871730 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/checkbox.cpython-312.pyc
--rw-r--r--   0        0        0     1311 2024-03-06 06:52:35.091364 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/checkbox.cpython-38.pyc
--rw-r--r--   0        0        0     2698 2024-03-26 02:40:10.840416 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form.cpython-312.pyc
--rw-r--r--   0        0        0     1888 2024-03-06 06:52:35.091364 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0      941 2024-03-25 08:58:16.987228 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form_item.cpython-312.pyc
--rw-r--r--   0        0        0      750 2024-03-06 06:52:35.091364 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form_item.cpython-38.pyc
--rw-r--r--   0        0        0     1718 2024-05-15 10:29:28.873271 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/input.cpython-312.pyc
--rw-r--r--   0        0        0      684 2024-03-06 06:52:35.091364 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/input.cpython-38.pyc
--rw-r--r--   0        0        0      714 2024-03-25 08:58:16.991228 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/message.cpython-312.pyc
--rw-r--r--   0        0        0      616 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/message.cpython-38.pyc
--rw-r--r--   0        0        0     1071 2024-03-26 07:34:45.962063 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/modal.cpython-312.pyc
--rw-r--r--   0        0        0      750 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/modal.cpython-38.pyc
--rw-r--r--   0        0        0     1402 2024-03-25 08:58:16.995228 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/page.cpython-312.pyc
--rw-r--r--   0        0        0     1037 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/page.cpython-38.pyc
--rw-r--r--   0        0        0     1427 2024-03-26 02:40:10.844416 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-312.pyc
--rw-r--r--   0        0        0     1121 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-38.pyc
--rw-r--r--   0        0        0     2492 2024-05-21 02:05:48.218160 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/row.cpython-312.pyc
--rw-r--r--   0        0        0     1850 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/row.cpython-38.pyc
--rw-r--r--   0        0        0     1283 2024-03-26 02:40:10.840416 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/select.cpython-312.pyc
--rw-r--r--   0        0        0      954 2024-03-06 06:52:35.091364 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/select.cpython-38.pyc
--rw-r--r--   0        0        0      435 2024-03-26 02:40:10.844416 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/spin.cpython-312.pyc
--rw-r--r--   0        0        0      445 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/spin.cpython-38.pyc
--rw-r--r--   0        0        0     1231 2024-03-27 09:06:08.774300 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/switch.cpython-312.pyc
--rw-r--r--   0        0        0     1059 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/switch.cpython-38.pyc
--rw-r--r--   0        0        0      689 2024-05-21 02:44:50.395485 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/tab.cpython-312.pyc
--rw-r--r--   0        0        0     2912 2024-05-21 06:49:20.526571 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/table.cpython-312.pyc
--rw-r--r--   0        0        0     1878 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/table.cpython-38.pyc
--rw-r--r--   0        0        0      432 2024-03-26 02:40:10.844416 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/text_area.cpython-312.pyc
--rw-r--r--   0        0        0      445 2024-03-06 06:52:35.095365 transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/text_area.cpython-38.pyc
--rw-r--r--   0        0        0      218 2024-03-27 08:37:01.671702 transstellar_antd-0.8.1/src/transstellar_antd/components/anchor.py
--rw-r--r--   0        0        0      136 2024-05-21 02:39:01.888576 transstellar_antd-0.8.1/src/transstellar_antd/components/breadcrumb.py
--rw-r--r--   0        0        0      252 2024-03-25 09:53:33.449454 transstellar_antd-0.8.1/src/transstellar_antd/components/button.py
--rw-r--r--   0        0        0     1189 2024-05-14 09:46:13.179723 transstellar_antd-0.8.1/src/transstellar_antd/components/checkbox.py
--rw-r--r--   0        0        0     1571 2024-03-26 02:35:00.099740 transstellar_antd-0.8.1/src/transstellar_antd/components/form.py
--rw-r--r--   0        0        0      406 2024-03-15 08:51:23.428684 transstellar_antd-0.8.1/src/transstellar_antd/components/form_item.py
--rw-r--r--   0        0        0      746 2024-05-15 10:24:38.209589 transstellar_antd-0.8.1/src/transstellar_antd/components/input.py
--rw-r--r--   0        0        0      242 2024-03-18 09:48:20.442505 transstellar_antd-0.8.1/src/transstellar_antd/components/message.py
--rw-r--r--   0        0        0      477 2024-03-26 07:33:39.677803 transstellar_antd-0.8.1/src/transstellar_antd/components/modal.py
--rw-r--r--   0        0        0      711 2024-03-20 03:39:46.144150 transstellar_antd-0.8.1/src/transstellar_antd/components/page.py
--rw-r--r--   0        0        0      719 2024-03-26 02:38:39.798952 transstellar_antd-0.8.1/src/transstellar_antd/components/popover_confirm.py
--rw-r--r--   0        0        0     1320 2024-05-21 02:05:46.142172 transstellar_antd-0.8.1/src/transstellar_antd/components/row.py
--rw-r--r--   0        0        0      685 2024-03-26 02:38:45.099092 transstellar_antd-0.8.1/src/transstellar_antd/components/select.py
--rw-r--r--   0        0        0      125 2024-03-26 02:38:47.587159 transstellar_antd-0.8.1/src/transstellar_antd/components/spin.py
--rw-r--r--   0        0        0      751 2024-03-27 09:05:58.406323 transstellar_antd-0.8.1/src/transstellar_antd/components/switch.py
--rw-r--r--   0        0        0      247 2024-05-21 02:41:56.694196 transstellar_antd-0.8.1/src/transstellar_antd/components/tab.py
--rw-r--r--   0        0        0     1808 2024-05-21 06:48:57.742536 transstellar_antd-0.8.1/src/transstellar_antd/components/table.py
--rw-r--r--   0        0        0      114 2024-03-26 02:38:57.295431 transstellar_antd-0.8.1/src/transstellar_antd/components/text_area.py
--rw-r--r--   0        0        0      967 2024-05-21 02:43:19.034841 transstellar_antd-0.8.1/src/transstellar_antd/v4/__init__.py
--rw-r--r--   0        0        0     1160 2024-05-21 02:44:50.395485 transstellar_antd-0.8.1/src/transstellar_antd/v4/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      267 2024-03-14 07:40:46.899468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      386 2024-05-21 02:37:39.291662 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/breadcrumb.cpython-312.pyc
--rw-r--r--   0        0        0      374 2024-03-26 10:08:38.901402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/button.cpython-312.pyc
--rw-r--r--   0        0        0      795 2024-03-14 07:40:46.899468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0      380 2024-03-26 10:08:38.901402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/checkbox.cpython-312.pyc
--rw-r--r--   0        0        0     1311 2024-03-14 07:40:46.903468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/checkbox.cpython-38.pyc
--rw-r--r--   0        0        0      757 2024-03-26 10:08:38.901402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form.cpython-312.pyc
--rw-r--r--   0        0        0     1888 2024-03-14 07:40:46.903468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0      381 2024-03-26 10:08:38.901402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form_item.cpython-312.pyc
--rw-r--r--   0        0        0      750 2024-03-14 07:40:46.903468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form_item.cpython-38.pyc
--rw-r--r--   0        0        0      371 2024-03-26 10:08:38.901402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/input.cpython-312.pyc
--rw-r--r--   0        0        0      684 2024-03-14 07:40:46.907468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/input.cpython-38.pyc
--rw-r--r--   0        0        0      435 2024-03-27 06:38:13.266884 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/message.cpython-312.pyc
--rw-r--r--   0        0        0      616 2024-03-14 07:40:46.907468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/message.cpython-38.pyc
--rw-r--r--   0        0        0      371 2024-03-26 10:08:38.905402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/modal.cpython-312.pyc
--rw-r--r--   0        0        0      750 2024-03-14 07:40:46.911468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/modal.cpython-38.pyc
--rw-r--r--   0        0        0      442 2024-03-26 10:08:38.905402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/page.cpython-312.pyc
--rw-r--r--   0        0        0     1037 2024-03-14 07:40:46.911468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/page.cpython-38.pyc
--rw-r--r--   0        0        0      471 2024-03-26 10:08:38.909402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/popover_confirm.cpython-312.pyc
--rw-r--r--   0        0        0     1121 2024-03-14 07:40:46.915468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/popover_confirm.cpython-38.pyc
--rw-r--r--   0        0        0      365 2024-03-26 10:08:38.909402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/row.cpython-312.pyc
--rw-r--r--   0        0        0     1850 2024-03-14 07:40:46.915468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/row.cpython-38.pyc
--rw-r--r--   0        0        0      374 2024-03-26 10:08:38.901402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/select.cpython-312.pyc
--rw-r--r--   0        0        0      954 2024-03-14 07:40:46.919468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/select.cpython-38.pyc
--rw-r--r--   0        0        0      368 2024-03-26 10:08:38.909402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/spin.cpython-312.pyc
--rw-r--r--   0        0        0      445 2024-03-14 07:40:46.919468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/spin.cpython-38.pyc
--rw-r--r--   0        0        0      374 2024-03-26 10:08:38.905402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/switch.cpython-312.pyc
--rw-r--r--   0        0        0     1059 2024-03-14 07:40:46.923468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/switch.cpython-38.pyc
--rw-r--r--   0        0        0      365 2024-05-21 02:44:50.399485 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/tab.cpython-312.pyc
--rw-r--r--   0        0        0      430 2024-05-21 02:44:50.399485 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/table.cpython-312.pyc
--rw-r--r--   0        0        0     1878 2024-03-14 07:40:46.923468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/table.cpython-38.pyc
--rw-r--r--   0        0        0      381 2024-03-26 10:08:38.905402 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/text_area.cpython-312.pyc
--rw-r--r--   0        0        0      445 2024-03-14 07:40:46.923468 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/text_area.cpython-38.pyc
--rw-r--r--   0        0        0      100 2024-05-21 02:36:09.054527 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/breadcrumb.py
--rw-r--r--   0        0        0       84 2024-03-14 08:22:01.993704 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/button.py
--rw-r--r--   0        0        0       92 2024-03-14 07:49:16.773015 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/checkbox.py
--rw-r--r--   0        0        0      388 2024-03-14 09:03:51.432408 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/form.py
--rw-r--r--   0        0        0       92 2024-03-14 07:49:19.221063 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/form_item.py
--rw-r--r--   0        0        0       80 2024-03-14 07:49:24.717170 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/input.py
--rw-r--r--   0        0        0      137 2024-03-27 06:31:28.879097 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/message.py
--rw-r--r--   0        0        0       80 2024-03-14 07:49:29.873271 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/modal.py
--rw-r--r--   0        0        0      134 2024-03-14 09:04:09.640442 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/page.py
--rw-r--r--   0        0        0      170 2024-03-14 09:04:29.676480 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/popover_confirm.py
--rw-r--r--   0        0        0       72 2024-03-14 07:50:12.418103 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/row.py
--rw-r--r--   0        0        0       84 2024-03-14 07:50:35.462556 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/select.py
--rw-r--r--   0        0        0       76 2024-03-14 07:51:03.959117 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/spin.py
--rw-r--r--   0        0        0       84 2024-03-14 07:51:23.211496 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/switch.py
--rw-r--r--   0        0        0       72 2024-05-21 02:43:01.562709 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/tab.py
--rw-r--r--   0        0        0      112 2024-05-21 02:42:42.786565 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/table.py
--rw-r--r--   0        0        0       92 2024-03-14 09:07:08.892808 transstellar_antd-0.8.1/src/transstellar_antd/v4/components/text_area.py
--rw-r--r--   0        0        0      967 2024-05-21 02:43:52.079082 transstellar_antd-0.8.1/src/transstellar_antd/v5/__init__.py
--rw-r--r--   0        0        0     1160 2024-05-21 02:44:50.399485 transstellar_antd-0.8.1/src/transstellar_antd/v5/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      267 2024-03-14 07:52:12.076463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      386 2024-05-21 02:39:34.452908 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/breadcrumb.cpython-312.pyc
--rw-r--r--   0        0        0      374 2024-03-25 08:58:16.999229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/button.cpython-312.pyc
--rw-r--r--   0        0        0      795 2024-03-14 07:52:12.076463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0      380 2024-03-25 08:58:16.999229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/checkbox.cpython-312.pyc
--rw-r--r--   0        0        0     1311 2024-03-14 07:52:12.076463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/checkbox.cpython-38.pyc
--rw-r--r--   0        0        0      757 2024-03-25 08:58:16.999229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form.cpython-312.pyc
--rw-r--r--   0        0        0     1888 2024-03-14 07:52:12.080463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form.cpython-38.pyc
--rw-r--r--   0        0        0      381 2024-03-25 08:58:16.999229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form_item.cpython-312.pyc
--rw-r--r--   0        0        0      750 2024-03-14 07:52:12.080463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form_item.cpython-38.pyc
--rw-r--r--   0        0        0      371 2024-03-25 08:58:17.003229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/input.cpython-312.pyc
--rw-r--r--   0        0        0      684 2024-03-14 07:52:12.080463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/input.cpython-38.pyc
--rw-r--r--   0        0        0      377 2024-03-27 06:28:54.975178 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/message.cpython-312.pyc
--rw-r--r--   0        0        0      616 2024-03-14 07:52:12.080463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/message.cpython-38.pyc
--rw-r--r--   0        0        0      371 2024-03-25 08:58:17.003229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/modal.cpython-312.pyc
--rw-r--r--   0        0        0      750 2024-03-14 07:52:12.080463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/modal.cpython-38.pyc
--rw-r--r--   0        0        0      439 2024-03-26 08:05:30.692170 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/page.cpython-312.pyc
--rw-r--r--   0        0        0     1037 2024-03-14 07:52:12.084463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/page.cpython-38.pyc
--rw-r--r--   0        0        0      468 2024-03-26 08:29:39.704703 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/popover_confirm.cpython-312.pyc
--rw-r--r--   0        0        0     1121 2024-03-14 07:52:12.084463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/popover_confirm.cpython-38.pyc
--rw-r--r--   0        0        0      365 2024-03-25 08:58:17.007228 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/row.cpython-312.pyc
--rw-r--r--   0        0        0     1850 2024-03-14 07:52:12.084463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/row.cpython-38.pyc
--rw-r--r--   0        0        0      374 2024-03-25 08:58:17.003229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/select.cpython-312.pyc
--rw-r--r--   0        0        0      954 2024-03-14 07:52:12.084463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/select.cpython-38.pyc
--rw-r--r--   0        0        0      368 2024-03-25 08:58:17.007228 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/spin.cpython-312.pyc
--rw-r--r--   0        0        0      445 2024-03-14 07:52:12.088463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/spin.cpython-38.pyc
--rw-r--r--   0        0        0      374 2024-03-25 08:58:17.003229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/switch.cpython-312.pyc
--rw-r--r--   0        0        0     1059 2024-03-14 07:52:12.088463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/switch.cpython-38.pyc
--rw-r--r--   0        0        0      365 2024-05-21 02:44:50.403485 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/tab.cpython-312.pyc
--rw-r--r--   0        0        0      433 2024-03-25 08:58:17.007228 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/table.cpython-312.pyc
--rw-r--r--   0        0        0     1878 2024-03-14 07:52:12.088463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/table.cpython-38.pyc
--rw-r--r--   0        0        0      381 2024-03-25 08:58:17.003229 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/text_area.cpython-312.pyc
--rw-r--r--   0        0        0      445 2024-03-14 07:52:12.088463 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/text_area.cpython-38.pyc
--rw-r--r--   0        0        0      100 2024-05-21 02:36:17.054634 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/breadcrumb.py
--rw-r--r--   0        0        0       84 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/button.py
--rw-r--r--   0        0        0       92 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/checkbox.py
--rw-r--r--   0        0        0      388 2024-03-14 09:07:56.908892 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/form.py
--rw-r--r--   0        0        0       92 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/form_item.py
--rw-r--r--   0        0        0       80 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/input.py
--rw-r--r--   0        0        0       88 2024-03-27 06:28:52.803179 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/message.py
--rw-r--r--   0        0        0       80 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/modal.py
--rw-r--r--   0        0        0      124 2024-03-26 08:04:20.024185 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/page.py
--rw-r--r--   0        0        0      160 2024-03-26 08:27:37.648322 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/popover_confirm.py
--rw-r--r--   0        0        0       72 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/row.py
--rw-r--r--   0        0        0       84 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/select.py
--rw-r--r--   0        0        0       76 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/spin.py
--rw-r--r--   0        0        0       84 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/switch.py
--rw-r--r--   0        0        0       72 2024-05-21 02:43:29.178916 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/tab.py
--rw-r--r--   0        0        0      122 2024-03-14 09:08:23.096807 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/table.py
--rw-r--r--   0        0        0       92 2024-03-14 08:23:02.933859 transstellar_antd-0.8.1/src/transstellar_antd/v5/components/text_area.py
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 transstellar_antd-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      388 2024-05-27 06:59:37.117663 transstellar_antd-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      923 2024-05-21 02:37:34.091601 transstellar_antd-0.9.0/src/transstellar_antd/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-27 03:29:14.748742 transstellar_antd-0.9.0/src/transstellar_antd/components/__init__.py
+-rw-r--r--   0        0        0      963 2024-05-27 03:30:30.893456 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      267 2024-02-27 04:17:55.380208 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      810 2024-03-27 08:44:31.501813 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/anchor.cpython-312.pyc
+-rw-r--r--   0        0        0      632 2024-05-27 06:46:42.292933 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/badge.cpython-312.pyc
+-rw-r--r--   0        0        0      454 2024-05-21 02:39:34.444908 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/breadcrumb.cpython-312.pyc
+-rw-r--r--   0        0        0      844 2024-03-25 09:53:39.649429 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/button.cpython-312.pyc
+-rw-r--r--   0        0        0      795 2024-03-06 06:52:35.091364 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0     1868 2024-05-14 09:46:23.871730 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     1311 2024-03-06 06:52:35.091364 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/checkbox.cpython-38.pyc
+-rw-r--r--   0        0        0     2698 2024-03-26 02:40:10.840416 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form.cpython-312.pyc
+-rw-r--r--   0        0        0     1888 2024-03-06 06:52:35.091364 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0      941 2024-03-25 08:58:16.987228 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form_item.cpython-312.pyc
+-rw-r--r--   0        0        0      750 2024-03-06 06:52:35.091364 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form_item.cpython-38.pyc
+-rw-r--r--   0        0        0     1718 2024-05-15 10:29:28.873271 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/input.cpython-312.pyc
+-rw-r--r--   0        0        0      684 2024-03-06 06:52:35.091364 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/input.cpython-38.pyc
+-rw-r--r--   0        0        0      714 2024-03-25 08:58:16.991228 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/message.cpython-312.pyc
+-rw-r--r--   0        0        0      616 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/message.cpython-38.pyc
+-rw-r--r--   0        0        0     1071 2024-03-26 07:34:45.962063 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/modal.cpython-312.pyc
+-rw-r--r--   0        0        0      750 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/modal.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2024-03-25 08:58:16.995228 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/page.cpython-312.pyc
+-rw-r--r--   0        0        0     1037 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0        0        0     1427 2024-03-26 02:40:10.844416 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-312.pyc
+-rw-r--r--   0        0        0     1121 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-38.pyc
+-rw-r--r--   0        0        0     2492 2024-05-21 02:05:48.218160 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/row.cpython-312.pyc
+-rw-r--r--   0        0        0     1850 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/row.cpython-38.pyc
+-rw-r--r--   0        0        0     1283 2024-03-26 02:40:10.840416 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/select.cpython-312.pyc
+-rw-r--r--   0        0        0      954 2024-03-06 06:52:35.091364 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/select.cpython-38.pyc
+-rw-r--r--   0        0        0      435 2024-03-26 02:40:10.844416 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/spin.cpython-312.pyc
+-rw-r--r--   0        0        0      445 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/spin.cpython-38.pyc
+-rw-r--r--   0        0        0     1231 2024-03-27 09:06:08.774300 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/switch.cpython-312.pyc
+-rw-r--r--   0        0        0     1059 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/switch.cpython-38.pyc
+-rw-r--r--   0        0        0      689 2024-05-21 02:44:50.395485 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/tab.cpython-312.pyc
+-rw-r--r--   0        0        0     3245 2024-05-27 03:24:59.938673 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/table.cpython-312.pyc
+-rw-r--r--   0        0        0     1878 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/table.cpython-38.pyc
+-rw-r--r--   0        0        0      432 2024-03-26 02:40:10.844416 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/text_area.cpython-312.pyc
+-rw-r--r--   0        0        0      445 2024-03-06 06:52:35.095365 transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/text_area.cpython-38.pyc
+-rw-r--r--   0        0        0      218 2024-03-27 08:37:01.671702 transstellar_antd-0.9.0/src/transstellar_antd/components/anchor.py
+-rw-r--r--   0        0        0      182 2024-05-27 06:46:38.272895 transstellar_antd-0.9.0/src/transstellar_antd/components/badge.py
+-rw-r--r--   0        0        0      136 2024-05-21 02:39:01.888576 transstellar_antd-0.9.0/src/transstellar_antd/components/breadcrumb.py
+-rw-r--r--   0        0        0      252 2024-03-25 09:53:33.449454 transstellar_antd-0.9.0/src/transstellar_antd/components/button.py
+-rw-r--r--   0        0        0     1189 2024-05-14 09:46:13.179723 transstellar_antd-0.9.0/src/transstellar_antd/components/checkbox.py
+-rw-r--r--   0        0        0     1571 2024-03-26 02:35:00.099740 transstellar_antd-0.9.0/src/transstellar_antd/components/form.py
+-rw-r--r--   0        0        0      406 2024-03-15 08:51:23.428684 transstellar_antd-0.9.0/src/transstellar_antd/components/form_item.py
+-rw-r--r--   0        0        0      746 2024-05-15 10:24:38.209589 transstellar_antd-0.9.0/src/transstellar_antd/components/input.py
+-rw-r--r--   0        0        0      242 2024-03-18 09:48:20.442505 transstellar_antd-0.9.0/src/transstellar_antd/components/message.py
+-rw-r--r--   0        0        0      477 2024-03-26 07:33:39.677803 transstellar_antd-0.9.0/src/transstellar_antd/components/modal.py
+-rw-r--r--   0        0        0      711 2024-03-20 03:39:46.144150 transstellar_antd-0.9.0/src/transstellar_antd/components/page.py
+-rw-r--r--   0        0        0      719 2024-03-26 02:38:39.798952 transstellar_antd-0.9.0/src/transstellar_antd/components/popover_confirm.py
+-rw-r--r--   0        0        0     1320 2024-05-21 02:05:46.142172 transstellar_antd-0.9.0/src/transstellar_antd/components/row.py
+-rw-r--r--   0        0        0      685 2024-03-26 02:38:45.099092 transstellar_antd-0.9.0/src/transstellar_antd/components/select.py
+-rw-r--r--   0        0        0      125 2024-03-26 02:38:47.587159 transstellar_antd-0.9.0/src/transstellar_antd/components/spin.py
+-rw-r--r--   0        0        0      751 2024-03-27 09:05:58.406323 transstellar_antd-0.9.0/src/transstellar_antd/components/switch.py
+-rw-r--r--   0        0        0      247 2024-05-21 02:41:56.694196 transstellar_antd-0.9.0/src/transstellar_antd/components/tab.py
+-rw-r--r--   0        0        0     1995 2024-05-27 03:24:55.302643 transstellar_antd-0.9.0/src/transstellar_antd/components/table.py
+-rw-r--r--   0        0        0      114 2024-03-26 02:38:57.295431 transstellar_antd-0.9.0/src/transstellar_antd/components/text_area.py
+-rw-r--r--   0        0        0     1016 2024-05-27 03:48:26.620497 transstellar_antd-0.9.0/src/transstellar_antd/v4/__init__.py
+-rw-r--r--   0        0        0     1212 2024-05-27 03:48:38.264568 transstellar_antd-0.9.0/src/transstellar_antd/v4/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      267 2024-03-14 07:40:46.899468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      371 2024-05-27 03:48:38.264568 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/badge.cpython-312.pyc
+-rw-r--r--   0        0        0      386 2024-05-21 02:37:39.291662 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/breadcrumb.cpython-312.pyc
+-rw-r--r--   0        0        0      374 2024-03-26 10:08:38.901402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/button.cpython-312.pyc
+-rw-r--r--   0        0        0      795 2024-03-14 07:40:46.899468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0      380 2024-03-26 10:08:38.901402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     1311 2024-03-14 07:40:46.903468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/checkbox.cpython-38.pyc
+-rw-r--r--   0        0        0      757 2024-03-26 10:08:38.901402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form.cpython-312.pyc
+-rw-r--r--   0        0        0     1888 2024-03-14 07:40:46.903468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0      381 2024-03-26 10:08:38.901402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form_item.cpython-312.pyc
+-rw-r--r--   0        0        0      750 2024-03-14 07:40:46.903468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form_item.cpython-38.pyc
+-rw-r--r--   0        0        0      371 2024-03-26 10:08:38.901402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/input.cpython-312.pyc
+-rw-r--r--   0        0        0      684 2024-03-14 07:40:46.907468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/input.cpython-38.pyc
+-rw-r--r--   0        0        0      435 2024-03-27 06:38:13.266884 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/message.cpython-312.pyc
+-rw-r--r--   0        0        0      616 2024-03-14 07:40:46.907468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/message.cpython-38.pyc
+-rw-r--r--   0        0        0      371 2024-03-26 10:08:38.905402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/modal.cpython-312.pyc
+-rw-r--r--   0        0        0      750 2024-03-14 07:40:46.911468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/modal.cpython-38.pyc
+-rw-r--r--   0        0        0      442 2024-03-26 10:08:38.905402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/page.cpython-312.pyc
+-rw-r--r--   0        0        0     1037 2024-03-14 07:40:46.911468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0        0        0      471 2024-03-26 10:08:38.909402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/popover_confirm.cpython-312.pyc
+-rw-r--r--   0        0        0     1121 2024-03-14 07:40:46.915468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/popover_confirm.cpython-38.pyc
+-rw-r--r--   0        0        0      365 2024-03-26 10:08:38.909402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/row.cpython-312.pyc
+-rw-r--r--   0        0        0     1850 2024-03-14 07:40:46.915468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/row.cpython-38.pyc
+-rw-r--r--   0        0        0      374 2024-03-26 10:08:38.901402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/select.cpython-312.pyc
+-rw-r--r--   0        0        0      954 2024-03-14 07:40:46.919468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/select.cpython-38.pyc
+-rw-r--r--   0        0        0      368 2024-03-26 10:08:38.909402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/spin.cpython-312.pyc
+-rw-r--r--   0        0        0      445 2024-03-14 07:40:46.919468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/spin.cpython-38.pyc
+-rw-r--r--   0        0        0      374 2024-03-26 10:08:38.905402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/switch.cpython-312.pyc
+-rw-r--r--   0        0        0     1059 2024-03-14 07:40:46.923468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/switch.cpython-38.pyc
+-rw-r--r--   0        0        0      365 2024-05-21 02:44:50.399485 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/tab.cpython-312.pyc
+-rw-r--r--   0        0        0      430 2024-05-21 02:44:50.399485 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/table.cpython-312.pyc
+-rw-r--r--   0        0        0     1878 2024-03-14 07:40:46.923468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/table.cpython-38.pyc
+-rw-r--r--   0        0        0      381 2024-03-26 10:08:38.905402 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/text_area.cpython-312.pyc
+-rw-r--r--   0        0        0      445 2024-03-14 07:40:46.923468 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/text_area.cpython-38.pyc
+-rw-r--r--   0        0        0       80 2024-05-27 03:29:48.917059 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/badge.py
+-rw-r--r--   0        0        0      100 2024-05-21 02:36:09.054527 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/breadcrumb.py
+-rw-r--r--   0        0        0       84 2024-03-14 08:22:01.993704 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/button.py
+-rw-r--r--   0        0        0       92 2024-03-14 07:49:16.773015 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/checkbox.py
+-rw-r--r--   0        0        0      388 2024-03-14 09:03:51.432408 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/form.py
+-rw-r--r--   0        0        0       92 2024-03-14 07:49:19.221063 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/form_item.py
+-rw-r--r--   0        0        0       80 2024-03-14 07:49:24.717170 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/input.py
+-rw-r--r--   0        0        0      137 2024-03-27 06:31:28.879097 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/message.py
+-rw-r--r--   0        0        0       80 2024-03-14 07:49:29.873271 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/modal.py
+-rw-r--r--   0        0        0      134 2024-03-14 09:04:09.640442 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/page.py
+-rw-r--r--   0        0        0      170 2024-03-14 09:04:29.676480 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/popover_confirm.py
+-rw-r--r--   0        0        0       72 2024-03-14 07:50:12.418103 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/row.py
+-rw-r--r--   0        0        0       84 2024-03-14 07:50:35.462556 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/select.py
+-rw-r--r--   0        0        0       76 2024-03-14 07:51:03.959117 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/spin.py
+-rw-r--r--   0        0        0       84 2024-03-14 07:51:23.211496 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/switch.py
+-rw-r--r--   0        0        0       72 2024-05-21 02:43:01.562709 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/tab.py
+-rw-r--r--   0        0        0      112 2024-05-21 02:42:42.786565 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/table.py
+-rw-r--r--   0        0        0       92 2024-03-14 09:07:08.892808 transstellar_antd-0.9.0/src/transstellar_antd/v4/components/text_area.py
+-rw-r--r--   0        0        0     1016 2024-05-27 03:48:13.028415 transstellar_antd-0.9.0/src/transstellar_antd/v5/__init__.py
+-rw-r--r--   0        0        0     1212 2024-05-27 03:48:38.272568 transstellar_antd-0.9.0/src/transstellar_antd/v5/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      267 2024-03-14 07:52:12.076463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      371 2024-05-27 03:48:38.276568 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/badge.cpython-312.pyc
+-rw-r--r--   0        0        0      386 2024-05-21 02:39:34.452908 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/breadcrumb.cpython-312.pyc
+-rw-r--r--   0        0        0      374 2024-03-25 08:58:16.999229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/button.cpython-312.pyc
+-rw-r--r--   0        0        0      795 2024-03-14 07:52:12.076463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0      380 2024-03-25 08:58:16.999229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     1311 2024-03-14 07:52:12.076463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/checkbox.cpython-38.pyc
+-rw-r--r--   0        0        0      757 2024-03-25 08:58:16.999229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form.cpython-312.pyc
+-rw-r--r--   0        0        0     1888 2024-03-14 07:52:12.080463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form.cpython-38.pyc
+-rw-r--r--   0        0        0      381 2024-03-25 08:58:16.999229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form_item.cpython-312.pyc
+-rw-r--r--   0        0        0      750 2024-03-14 07:52:12.080463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form_item.cpython-38.pyc
+-rw-r--r--   0        0        0      371 2024-03-25 08:58:17.003229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/input.cpython-312.pyc
+-rw-r--r--   0        0        0      684 2024-03-14 07:52:12.080463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/input.cpython-38.pyc
+-rw-r--r--   0        0        0      377 2024-03-27 06:28:54.975178 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/message.cpython-312.pyc
+-rw-r--r--   0        0        0      616 2024-03-14 07:52:12.080463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/message.cpython-38.pyc
+-rw-r--r--   0        0        0      371 2024-03-25 08:58:17.003229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/modal.cpython-312.pyc
+-rw-r--r--   0        0        0      750 2024-03-14 07:52:12.080463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/modal.cpython-38.pyc
+-rw-r--r--   0        0        0      439 2024-03-26 08:05:30.692170 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/page.cpython-312.pyc
+-rw-r--r--   0        0        0     1037 2024-03-14 07:52:12.084463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/page.cpython-38.pyc
+-rw-r--r--   0        0        0      468 2024-03-26 08:29:39.704703 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/popover_confirm.cpython-312.pyc
+-rw-r--r--   0        0        0     1121 2024-03-14 07:52:12.084463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/popover_confirm.cpython-38.pyc
+-rw-r--r--   0        0        0      365 2024-03-25 08:58:17.007228 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/row.cpython-312.pyc
+-rw-r--r--   0        0        0     1850 2024-03-14 07:52:12.084463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/row.cpython-38.pyc
+-rw-r--r--   0        0        0      374 2024-03-25 08:58:17.003229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/select.cpython-312.pyc
+-rw-r--r--   0        0        0      954 2024-03-14 07:52:12.084463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/select.cpython-38.pyc
+-rw-r--r--   0        0        0      368 2024-03-25 08:58:17.007228 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/spin.cpython-312.pyc
+-rw-r--r--   0        0        0      445 2024-03-14 07:52:12.088463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/spin.cpython-38.pyc
+-rw-r--r--   0        0        0      374 2024-03-25 08:58:17.003229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/switch.cpython-312.pyc
+-rw-r--r--   0        0        0     1059 2024-03-14 07:52:12.088463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/switch.cpython-38.pyc
+-rw-r--r--   0        0        0      365 2024-05-21 02:44:50.403485 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/tab.cpython-312.pyc
+-rw-r--r--   0        0        0      433 2024-03-25 08:58:17.007228 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/table.cpython-312.pyc
+-rw-r--r--   0        0        0     1878 2024-03-14 07:52:12.088463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/table.cpython-38.pyc
+-rw-r--r--   0        0        0      381 2024-03-25 08:58:17.003229 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/text_area.cpython-312.pyc
+-rw-r--r--   0        0        0      445 2024-03-14 07:52:12.088463 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/text_area.cpython-38.pyc
+-rw-r--r--   0        0        0       80 2024-05-27 03:29:57.825142 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/badge.py
+-rw-r--r--   0        0        0      100 2024-05-21 02:36:17.054634 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/breadcrumb.py
+-rw-r--r--   0        0        0       84 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/button.py
+-rw-r--r--   0        0        0       92 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/checkbox.py
+-rw-r--r--   0        0        0      388 2024-03-14 09:07:56.908892 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/form.py
+-rw-r--r--   0        0        0       92 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/form_item.py
+-rw-r--r--   0        0        0       80 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/input.py
+-rw-r--r--   0        0        0       88 2024-03-27 06:28:52.803179 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/message.py
+-rw-r--r--   0        0        0       80 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/modal.py
+-rw-r--r--   0        0        0      124 2024-03-26 08:04:20.024185 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/page.py
+-rw-r--r--   0        0        0      160 2024-03-26 08:27:37.648322 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/popover_confirm.py
+-rw-r--r--   0        0        0       72 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/row.py
+-rw-r--r--   0        0        0       84 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/select.py
+-rw-r--r--   0        0        0       76 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/spin.py
+-rw-r--r--   0        0        0       84 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/switch.py
+-rw-r--r--   0        0        0       72 2024-05-21 02:43:29.178916 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/tab.py
+-rw-r--r--   0        0        0      122 2024-03-14 09:08:23.096807 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/table.py
+-rw-r--r--   0        0        0       92 2024-03-14 08:23:02.933859 transstellar_antd-0.9.0/src/transstellar_antd/v5/components/text_area.py
+-rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 transstellar_antd-0.9.0/PKG-INFO
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/__init__.py` & `transstellar_antd-0.9.0/src/transstellar_antd/__init__.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__init__.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 __all__ = [
+    "Badge",
     "Button",
     "Breadcrumb",
     "Checkbox",
     "Form",
     "FormItem",
     "Input",
     "Message",
@@ -14,14 +15,15 @@
     "Spin",
     "Switch",
     "Tab",
     "Table",
     "TextArea",
 ]
 
+from .badge import Badge
 from .breadcrumb import Breadcrumb
 from .button import Button
 from .checkbox import Checkbox
 from .form import Form
 from .form_item import FormItem
 from .input import Input
 from .message import Message
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/__init__.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/__init__.cpython-312.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,153 +1,161 @@
 magic:    0xcb0d0d0a
-moddate:  0x0a0a4c66 (Tue May 21 02:42:18 2024 UTC)
-files sz: 727
+moddate:  0x0afe5366 (Mon May 27 03:29:14 2024 UTC)
+files sz: 765
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x970067006400a2015a00640164026c016d025a020100640164036c036d
       045a040100640164046c056d065a060100640164056c076d085a08010064
       0164066c096d0a5a0a0100640164076c0b6d0c5a0c0100640164086c0d6d
       0e5a0e0100640164096c0f6d105a1001006401640a6c116d125a12010064
       01640b6c136d145a1401006401640c6c156d165a1601006401640d6c176d
       185a1801006401640e6c196d1a5a1a01006401640f6c1b6d1c5a1c010064
       0164106c1d6d1e5a1e0100640164116c1f6d205a200100640164126c216d
-      225a220100a613
+      225a220100640164136c236d245a240100a614
      0           0 RESUME                   0
    
      1           2 BUILD_LIST               0
-                 4 LOAD_CONST               0 (('Button', 'Breadcrumb', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea'))
+                 4 LOAD_CONST               0 (('Badge', 'Button', 'Breadcrumb', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea'))
                  6 LIST_EXTEND              1
                  8 STORE_NAME               0 (__all__)
    
-    21          10 LOAD_CONST               1 (1)
-                12 LOAD_CONST               2 (('Breadcrumb',))
-                14 IMPORT_NAME              1 (breadcrumb)
-                16 IMPORT_FROM              2 (Breadcrumb)
-                18 STORE_NAME               2 (Breadcrumb)
+    22          10 LOAD_CONST               1 (1)
+                12 LOAD_CONST               2 (('Badge',))
+                14 IMPORT_NAME              1 (badge)
+                16 IMPORT_FROM              2 (Badge)
+                18 STORE_NAME               2 (Badge)
                 20 POP_TOP
    
-    22          22 LOAD_CONST               1 (1)
-                24 LOAD_CONST               3 (('Button',))
-                26 IMPORT_NAME              3 (button)
-                28 IMPORT_FROM              4 (Button)
-                30 STORE_NAME               4 (Button)
+    23          22 LOAD_CONST               1 (1)
+                24 LOAD_CONST               3 (('Breadcrumb',))
+                26 IMPORT_NAME              3 (breadcrumb)
+                28 IMPORT_FROM              4 (Breadcrumb)
+                30 STORE_NAME               4 (Breadcrumb)
                 32 POP_TOP
    
-    23          34 LOAD_CONST               1 (1)
-                36 LOAD_CONST               4 (('Checkbox',))
-                38 IMPORT_NAME              5 (checkbox)
-                40 IMPORT_FROM              6 (Checkbox)
-                42 STORE_NAME               6 (Checkbox)
+    24          34 LOAD_CONST               1 (1)
+                36 LOAD_CONST               4 (('Button',))
+                38 IMPORT_NAME              5 (button)
+                40 IMPORT_FROM              6 (Button)
+                42 STORE_NAME               6 (Button)
                 44 POP_TOP
    
-    24          46 LOAD_CONST               1 (1)
-                48 LOAD_CONST               5 (('Form',))
-                50 IMPORT_NAME              7 (form)
-                52 IMPORT_FROM              8 (Form)
-                54 STORE_NAME               8 (Form)
+    25          46 LOAD_CONST               1 (1)
+                48 LOAD_CONST               5 (('Checkbox',))
+                50 IMPORT_NAME              7 (checkbox)
+                52 IMPORT_FROM              8 (Checkbox)
+                54 STORE_NAME               8 (Checkbox)
                 56 POP_TOP
    
-    25          58 LOAD_CONST               1 (1)
-                60 LOAD_CONST               6 (('FormItem',))
-                62 IMPORT_NAME              9 (form_item)
-                64 IMPORT_FROM             10 (FormItem)
-                66 STORE_NAME              10 (FormItem)
+    26          58 LOAD_CONST               1 (1)
+                60 LOAD_CONST               6 (('Form',))
+                62 IMPORT_NAME              9 (form)
+                64 IMPORT_FROM             10 (Form)
+                66 STORE_NAME              10 (Form)
                 68 POP_TOP
    
-    26          70 LOAD_CONST               1 (1)
-                72 LOAD_CONST               7 (('Input',))
-                74 IMPORT_NAME             11 (input)
-                76 IMPORT_FROM             12 (Input)
-                78 STORE_NAME              12 (Input)
+    27          70 LOAD_CONST               1 (1)
+                72 LOAD_CONST               7 (('FormItem',))
+                74 IMPORT_NAME             11 (form_item)
+                76 IMPORT_FROM             12 (FormItem)
+                78 STORE_NAME              12 (FormItem)
                 80 POP_TOP
    
-    27          82 LOAD_CONST               1 (1)
-                84 LOAD_CONST               8 (('Message',))
-                86 IMPORT_NAME             13 (message)
-                88 IMPORT_FROM             14 (Message)
-                90 STORE_NAME              14 (Message)
+    28          82 LOAD_CONST               1 (1)
+                84 LOAD_CONST               8 (('Input',))
+                86 IMPORT_NAME             13 (input)
+                88 IMPORT_FROM             14 (Input)
+                90 STORE_NAME              14 (Input)
                 92 POP_TOP
    
-    28          94 LOAD_CONST               1 (1)
-                96 LOAD_CONST               9 (('Modal',))
-                98 IMPORT_NAME             15 (modal)
-               100 IMPORT_FROM             16 (Modal)
-               102 STORE_NAME              16 (Modal)
+    29          94 LOAD_CONST               1 (1)
+                96 LOAD_CONST               9 (('Message',))
+                98 IMPORT_NAME             15 (message)
+               100 IMPORT_FROM             16 (Message)
+               102 STORE_NAME              16 (Message)
                104 POP_TOP
    
-    29         106 LOAD_CONST               1 (1)
-               108 LOAD_CONST              10 (('Page',))
-               110 IMPORT_NAME             17 (page)
-               112 IMPORT_FROM             18 (Page)
-               114 STORE_NAME              18 (Page)
+    30         106 LOAD_CONST               1 (1)
+               108 LOAD_CONST              10 (('Modal',))
+               110 IMPORT_NAME             17 (modal)
+               112 IMPORT_FROM             18 (Modal)
+               114 STORE_NAME              18 (Modal)
                116 POP_TOP
    
-    30         118 LOAD_CONST               1 (1)
-               120 LOAD_CONST              11 (('PopoverConfirm',))
-               122 IMPORT_NAME             19 (popover_confirm)
-               124 IMPORT_FROM             20 (PopoverConfirm)
-               126 STORE_NAME              20 (PopoverConfirm)
+    31         118 LOAD_CONST               1 (1)
+               120 LOAD_CONST              11 (('Page',))
+               122 IMPORT_NAME             19 (page)
+               124 IMPORT_FROM             20 (Page)
+               126 STORE_NAME              20 (Page)
                128 POP_TOP
    
-    31         130 LOAD_CONST               1 (1)
-               132 LOAD_CONST              12 (('Row',))
-               134 IMPORT_NAME             21 (row)
-               136 IMPORT_FROM             22 (Row)
-               138 STORE_NAME              22 (Row)
+    32         130 LOAD_CONST               1 (1)
+               132 LOAD_CONST              12 (('PopoverConfirm',))
+               134 IMPORT_NAME             21 (popover_confirm)
+               136 IMPORT_FROM             22 (PopoverConfirm)
+               138 STORE_NAME              22 (PopoverConfirm)
                140 POP_TOP
    
-    32         142 LOAD_CONST               1 (1)
-               144 LOAD_CONST              13 (('Select',))
-               146 IMPORT_NAME             23 (select)
-               148 IMPORT_FROM             24 (Select)
-               150 STORE_NAME              24 (Select)
+    33         142 LOAD_CONST               1 (1)
+               144 LOAD_CONST              13 (('Row',))
+               146 IMPORT_NAME             23 (row)
+               148 IMPORT_FROM             24 (Row)
+               150 STORE_NAME              24 (Row)
                152 POP_TOP
    
-    33         154 LOAD_CONST               1 (1)
-               156 LOAD_CONST              14 (('Spin',))
-               158 IMPORT_NAME             25 (spin)
-               160 IMPORT_FROM             26 (Spin)
-               162 STORE_NAME              26 (Spin)
+    34         154 LOAD_CONST               1 (1)
+               156 LOAD_CONST              14 (('Select',))
+               158 IMPORT_NAME             25 (select)
+               160 IMPORT_FROM             26 (Select)
+               162 STORE_NAME              26 (Select)
                164 POP_TOP
    
-    34         166 LOAD_CONST               1 (1)
-               168 LOAD_CONST              15 (('Switch',))
-               170 IMPORT_NAME             27 (switch)
-               172 IMPORT_FROM             28 (Switch)
-               174 STORE_NAME              28 (Switch)
+    35         166 LOAD_CONST               1 (1)
+               168 LOAD_CONST              15 (('Spin',))
+               170 IMPORT_NAME             27 (spin)
+               172 IMPORT_FROM             28 (Spin)
+               174 STORE_NAME              28 (Spin)
                176 POP_TOP
    
-    35         178 LOAD_CONST               1 (1)
-               180 LOAD_CONST              16 (('Tab',))
-               182 IMPORT_NAME             29 (tab)
-               184 IMPORT_FROM             30 (Tab)
-               186 STORE_NAME              30 (Tab)
+    36         178 LOAD_CONST               1 (1)
+               180 LOAD_CONST              16 (('Switch',))
+               182 IMPORT_NAME             29 (switch)
+               184 IMPORT_FROM             30 (Switch)
+               186 STORE_NAME              30 (Switch)
                188 POP_TOP
    
-    36         190 LOAD_CONST               1 (1)
-               192 LOAD_CONST              17 (('Table',))
-               194 IMPORT_NAME             31 (table)
-               196 IMPORT_FROM             32 (Table)
-               198 STORE_NAME              32 (Table)
+    37         190 LOAD_CONST               1 (1)
+               192 LOAD_CONST              17 (('Tab',))
+               194 IMPORT_NAME             31 (tab)
+               196 IMPORT_FROM             32 (Tab)
+               198 STORE_NAME              32 (Tab)
                200 POP_TOP
    
-    37         202 LOAD_CONST               1 (1)
-               204 LOAD_CONST              18 (('TextArea',))
-               206 IMPORT_NAME             33 (text_area)
-               208 IMPORT_FROM             34 (TextArea)
-               210 STORE_NAME              34 (TextArea)
+    38         202 LOAD_CONST               1 (1)
+               204 LOAD_CONST              18 (('Table',))
+               206 IMPORT_NAME             33 (table)
+               208 IMPORT_FROM             34 (Table)
+               210 STORE_NAME              34 (Table)
                212 POP_TOP
-               214 PRECALL                 19
+   
+    39         214 LOAD_CONST               1 (1)
+               216 LOAD_CONST              19 (('TextArea',))
+               218 IMPORT_NAME             35 (text_area)
+               220 IMPORT_FROM             36 (TextArea)
+               222 STORE_NAME              36 (TextArea)
+               224 POP_TOP
+               226 PRECALL                 20
    consts
-      ('Button', 'Breadcrumb', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea')
+      ('Badge', 'Button', 'Breadcrumb', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea')
       1
+      ('Badge',)
       ('Breadcrumb',)
       ('Button',)
       ('Checkbox',)
       ('Form',)
       ('FormItem',)
       ('Input',)
       ('Message',)
@@ -158,17 +166,17 @@
       ('Select',)
       ('Spin',)
       ('Switch',)
       ('Tab',)
       ('Table',)
       ('TextArea',)
       None
-   names      ('__all__', 'breadcrumb', 'Breadcrumb', 'button', 'Button', 'checkbox', 'Checkbox', 'form', 'Form', 'form_item', 'FormItem', 'input', 'Input', 'message', 'Message', 'modal', 'Modal', 'page', 'Page', 'popover_confirm', 'PopoverConfirm', 'row', 'Row', 'select', 'Select', 'spin', 'Spin', 'switch', 'Switch', 'tab', 'Tab', 'table', 'Table', 'text_area', 'TextArea')
+   names      ('__all__', 'badge', 'Badge', 'breadcrumb', 'Breadcrumb', 'button', 'Button', 'checkbox', 'Checkbox', 'form', 'Form', 'form_item', 'FormItem', 'input', 'Input', 'message', 'Message', 'modal', 'Modal', 'page', 'Page', 'popover_confirm', 'PopoverConfirm', 'row', 'Row', 'select', 'Select', 'spin', 'Spin', 'switch', 'Switch', 'tab', 'Tab', 'table', 'Table', 'text_area', 'TextArea')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/project/src/transstellar_antd/components/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108140c010c010c010c010c010c010c010c010c010c010c010c
-      010c010c010c010c01
+      0x00ff020108150c010c010c010c010c010c010c010c010c010c010c010c
+      010c010c010c010c010c01
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/anchor.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/anchor.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/button.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/button.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/button.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/checkbox.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/checkbox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/checkbox.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/checkbox.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form_item.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form_item.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/form_item.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/form_item.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/input.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/input.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/input.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/input.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/message.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/message.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/message.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/modal.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/modal.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/modal.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/modal.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/page.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/page.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/page.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/popover_confirm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/row.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/row.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/row.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/row.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/select.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/select.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/select.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/select.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/switch.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/switch.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/switch.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/switch.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/tab.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/tab.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/__pycache__/table.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/components/__pycache__/table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/checkbox.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/form.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/form.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/input.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/input.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/page.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/page.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/popover_confirm.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/popover_confirm.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/row.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/row.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/select.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/select.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/switch.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/switch.py`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/components/table.py` & `transstellar_antd-0.9.0/src/transstellar_antd/components/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from selenium.webdriver.common.by import By
 from transstellar.framework import Element
 
 from .row import Row
 
 
 class Table(Element):
-    XPATH_CURRENT = '//div[contains(@class, "ant-table")]'
+    XPATH_CURRENT = '//div[contains(@class, "ant-table ")]'
     SELECTOR_TABLE_HEADER = "thead.ant-table-thead th.ant-table-cell"
     SELECTOR_ROW = "tbody.ant-table-tbody tr.ant-table-row"
     ROW_CLASS = Row
 
     rows: List[Row]
     column_titles = {}
 
@@ -25,18 +25,24 @@
 
             # Sometimes there is a column used as scrollbar
             if column_name == "":
                 continue
 
             self.column_titles[column_name] = index
 
-        self.rows = self.find_elements(self.ROW_CLASS)
+        if not self.is_empty():
+            self.rows = self.find_elements(self.ROW_CLASS)
 
-        for row in self.rows:
-            row.set_column_titles(self.column_titles)
+            for row in self.rows:
+                row.set_column_titles(self.column_titles)
+
+    def is_empty(self):
+        classes = self.get_current_dom_element().get_attribute("class")
+
+        return "ant-table-empty" in classes
 
     def find_row(self, column_title: str, column_text: str) -> Union[None, Row]:
         self.logger.info(f"finding row with column {column_title}: {column_text}")
 
         column_index = self.column_titles[column_title]
 
         if column_index is not None:
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/__init__.py` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = [
     "Anchor",
+    "Badge",
     "Breadcrumb",
     "Button",
     "Checkbox",
     "Form",
     "FormItem",
     "Input",
     "Message",
@@ -16,14 +17,15 @@
     "Switch",
     "Tab",
     "Table",
     "TextArea",
 ]
 
 from ..components.anchor import Anchor
+from .components.badge import Badge
 from .components.breadcrumb import Breadcrumb
 from .components.button import Button
 from .components.checkbox import Checkbox
 from .components.form import Form
 from .components.form_item import FormItem
 from .components.input import Input
 from .components.message import Message
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/__pycache__/__init__.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/__pycache__/__init__.cpython-312.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,162 +1,171 @@
 magic:    0xcb0d0d0a
-moddate:  0x470a4c66 (Tue May 21 02:43:19 2024 UTC)
-files sz: 967
+moddate:  0x8a025466 (Mon May 27 03:48:26 2024 UTC)
+files sz: 1016
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x970067006400a2015a00640164026c016d025a020100640364046c036d
       045a040100640364056c056d065a060100640364066c076d085a08010064
       0364076c096d0a5a0a0100640364086c0b6d0c5a0c0100640364096c0d6d
       0e5a0e01006403640a6c0f6d105a1001006403640b6c116d125a12010064
       03640c6c136d145a1401006403640d6c156d165a1601006403640e6c176d
       185a1801006403640f6c196d1a5a1a0100640364106c1b6d1c5a1c010064
       0364116c1d6d1e5a1e0100640364126c1f6d205a200100640364136c216d
-      225a220100640364146c236d245a240100a615
+      225a220100640364146c236d245a240100640364156c256d265a260100a6
+      16
      0           0 RESUME                   0
    
      1           2 BUILD_LIST               0
-                 4 LOAD_CONST               0 (('Anchor', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea'))
+                 4 LOAD_CONST               0 (('Anchor', 'Badge', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea'))
                  6 LIST_EXTEND              1
                  8 STORE_NAME               0 (__all__)
    
-    22          10 LOAD_CONST               1 (2)
+    23          10 LOAD_CONST               1 (2)
                 12 LOAD_CONST               2 (('Anchor',))
                 14 IMPORT_NAME              1 (components.anchor)
                 16 IMPORT_FROM              2 (Anchor)
                 18 STORE_NAME               2 (Anchor)
                 20 POP_TOP
    
-    23          22 LOAD_CONST               3 (1)
-                24 LOAD_CONST               4 (('Breadcrumb',))
-                26 IMPORT_NAME              3 (components.breadcrumb)
-                28 IMPORT_FROM              4 (Breadcrumb)
-                30 STORE_NAME               4 (Breadcrumb)
+    24          22 LOAD_CONST               3 (1)
+                24 LOAD_CONST               4 (('Badge',))
+                26 IMPORT_NAME              3 (components.badge)
+                28 IMPORT_FROM              4 (Badge)
+                30 STORE_NAME               4 (Badge)
                 32 POP_TOP
    
-    24          34 LOAD_CONST               3 (1)
-                36 LOAD_CONST               5 (('Button',))
-                38 IMPORT_NAME              5 (components.button)
-                40 IMPORT_FROM              6 (Button)
-                42 STORE_NAME               6 (Button)
+    25          34 LOAD_CONST               3 (1)
+                36 LOAD_CONST               5 (('Breadcrumb',))
+                38 IMPORT_NAME              5 (components.breadcrumb)
+                40 IMPORT_FROM              6 (Breadcrumb)
+                42 STORE_NAME               6 (Breadcrumb)
                 44 POP_TOP
    
-    25          46 LOAD_CONST               3 (1)
-                48 LOAD_CONST               6 (('Checkbox',))
-                50 IMPORT_NAME              7 (components.checkbox)
-                52 IMPORT_FROM              8 (Checkbox)
-                54 STORE_NAME               8 (Checkbox)
+    26          46 LOAD_CONST               3 (1)
+                48 LOAD_CONST               6 (('Button',))
+                50 IMPORT_NAME              7 (components.button)
+                52 IMPORT_FROM              8 (Button)
+                54 STORE_NAME               8 (Button)
                 56 POP_TOP
    
-    26          58 LOAD_CONST               3 (1)
-                60 LOAD_CONST               7 (('Form',))
-                62 IMPORT_NAME              9 (components.form)
-                64 IMPORT_FROM             10 (Form)
-                66 STORE_NAME              10 (Form)
+    27          58 LOAD_CONST               3 (1)
+                60 LOAD_CONST               7 (('Checkbox',))
+                62 IMPORT_NAME              9 (components.checkbox)
+                64 IMPORT_FROM             10 (Checkbox)
+                66 STORE_NAME              10 (Checkbox)
                 68 POP_TOP
    
-    27          70 LOAD_CONST               3 (1)
-                72 LOAD_CONST               8 (('FormItem',))
-                74 IMPORT_NAME             11 (components.form_item)
-                76 IMPORT_FROM             12 (FormItem)
-                78 STORE_NAME              12 (FormItem)
+    28          70 LOAD_CONST               3 (1)
+                72 LOAD_CONST               8 (('Form',))
+                74 IMPORT_NAME             11 (components.form)
+                76 IMPORT_FROM             12 (Form)
+                78 STORE_NAME              12 (Form)
                 80 POP_TOP
    
-    28          82 LOAD_CONST               3 (1)
-                84 LOAD_CONST               9 (('Input',))
-                86 IMPORT_NAME             13 (components.input)
-                88 IMPORT_FROM             14 (Input)
-                90 STORE_NAME              14 (Input)
+    29          82 LOAD_CONST               3 (1)
+                84 LOAD_CONST               9 (('FormItem',))
+                86 IMPORT_NAME             13 (components.form_item)
+                88 IMPORT_FROM             14 (FormItem)
+                90 STORE_NAME              14 (FormItem)
                 92 POP_TOP
    
-    29          94 LOAD_CONST               3 (1)
-                96 LOAD_CONST              10 (('Message',))
-                98 IMPORT_NAME             15 (components.message)
-               100 IMPORT_FROM             16 (Message)
-               102 STORE_NAME              16 (Message)
+    30          94 LOAD_CONST               3 (1)
+                96 LOAD_CONST              10 (('Input',))
+                98 IMPORT_NAME             15 (components.input)
+               100 IMPORT_FROM             16 (Input)
+               102 STORE_NAME              16 (Input)
                104 POP_TOP
    
-    30         106 LOAD_CONST               3 (1)
-               108 LOAD_CONST              11 (('Modal',))
-               110 IMPORT_NAME             17 (components.modal)
-               112 IMPORT_FROM             18 (Modal)
-               114 STORE_NAME              18 (Modal)
+    31         106 LOAD_CONST               3 (1)
+               108 LOAD_CONST              11 (('Message',))
+               110 IMPORT_NAME             17 (components.message)
+               112 IMPORT_FROM             18 (Message)
+               114 STORE_NAME              18 (Message)
                116 POP_TOP
    
-    31         118 LOAD_CONST               3 (1)
-               120 LOAD_CONST              12 (('Page',))
-               122 IMPORT_NAME             19 (components.page)
-               124 IMPORT_FROM             20 (Page)
-               126 STORE_NAME              20 (Page)
+    32         118 LOAD_CONST               3 (1)
+               120 LOAD_CONST              12 (('Modal',))
+               122 IMPORT_NAME             19 (components.modal)
+               124 IMPORT_FROM             20 (Modal)
+               126 STORE_NAME              20 (Modal)
                128 POP_TOP
    
-    32         130 LOAD_CONST               3 (1)
-               132 LOAD_CONST              13 (('PopoverConfirm',))
-               134 IMPORT_NAME             21 (components.popover_confirm)
-               136 IMPORT_FROM             22 (PopoverConfirm)
-               138 STORE_NAME              22 (PopoverConfirm)
+    33         130 LOAD_CONST               3 (1)
+               132 LOAD_CONST              13 (('Page',))
+               134 IMPORT_NAME             21 (components.page)
+               136 IMPORT_FROM             22 (Page)
+               138 STORE_NAME              22 (Page)
                140 POP_TOP
    
-    33         142 LOAD_CONST               3 (1)
-               144 LOAD_CONST              14 (('Row',))
-               146 IMPORT_NAME             23 (components.row)
-               148 IMPORT_FROM             24 (Row)
-               150 STORE_NAME              24 (Row)
+    34         142 LOAD_CONST               3 (1)
+               144 LOAD_CONST              14 (('PopoverConfirm',))
+               146 IMPORT_NAME             23 (components.popover_confirm)
+               148 IMPORT_FROM             24 (PopoverConfirm)
+               150 STORE_NAME              24 (PopoverConfirm)
                152 POP_TOP
    
-    34         154 LOAD_CONST               3 (1)
-               156 LOAD_CONST              15 (('Select',))
-               158 IMPORT_NAME             25 (components.select)
-               160 IMPORT_FROM             26 (Select)
-               162 STORE_NAME              26 (Select)
+    35         154 LOAD_CONST               3 (1)
+               156 LOAD_CONST              15 (('Row',))
+               158 IMPORT_NAME             25 (components.row)
+               160 IMPORT_FROM             26 (Row)
+               162 STORE_NAME              26 (Row)
                164 POP_TOP
    
-    35         166 LOAD_CONST               3 (1)
-               168 LOAD_CONST              16 (('Spin',))
-               170 IMPORT_NAME             27 (components.spin)
-               172 IMPORT_FROM             28 (Spin)
-               174 STORE_NAME              28 (Spin)
+    36         166 LOAD_CONST               3 (1)
+               168 LOAD_CONST              16 (('Select',))
+               170 IMPORT_NAME             27 (components.select)
+               172 IMPORT_FROM             28 (Select)
+               174 STORE_NAME              28 (Select)
                176 POP_TOP
    
-    36         178 LOAD_CONST               3 (1)
-               180 LOAD_CONST              17 (('Switch',))
-               182 IMPORT_NAME             29 (components.switch)
-               184 IMPORT_FROM             30 (Switch)
-               186 STORE_NAME              30 (Switch)
+    37         178 LOAD_CONST               3 (1)
+               180 LOAD_CONST              17 (('Spin',))
+               182 IMPORT_NAME             29 (components.spin)
+               184 IMPORT_FROM             30 (Spin)
+               186 STORE_NAME              30 (Spin)
                188 POP_TOP
    
-    37         190 LOAD_CONST               3 (1)
-               192 LOAD_CONST              18 (('Tab',))
-               194 IMPORT_NAME             31 (components.tab)
-               196 IMPORT_FROM             32 (Tab)
-               198 STORE_NAME              32 (Tab)
+    38         190 LOAD_CONST               3 (1)
+               192 LOAD_CONST              18 (('Switch',))
+               194 IMPORT_NAME             31 (components.switch)
+               196 IMPORT_FROM             32 (Switch)
+               198 STORE_NAME              32 (Switch)
                200 POP_TOP
    
-    38         202 LOAD_CONST               3 (1)
-               204 LOAD_CONST              19 (('Table',))
-               206 IMPORT_NAME             33 (components.table)
-               208 IMPORT_FROM             34 (Table)
-               210 STORE_NAME              34 (Table)
+    39         202 LOAD_CONST               3 (1)
+               204 LOAD_CONST              19 (('Tab',))
+               206 IMPORT_NAME             33 (components.tab)
+               208 IMPORT_FROM             34 (Tab)
+               210 STORE_NAME              34 (Tab)
                212 POP_TOP
    
-    39         214 LOAD_CONST               3 (1)
-               216 LOAD_CONST              20 (('TextArea',))
-               218 IMPORT_NAME             35 (components.text_area)
-               220 IMPORT_FROM             36 (TextArea)
-               222 STORE_NAME              36 (TextArea)
+    40         214 LOAD_CONST               3 (1)
+               216 LOAD_CONST              20 (('Table',))
+               218 IMPORT_NAME             35 (components.table)
+               220 IMPORT_FROM             36 (Table)
+               222 STORE_NAME              36 (Table)
                224 POP_TOP
-               226 PRECALL                 21
+   
+    41         226 LOAD_CONST               3 (1)
+               228 LOAD_CONST              21 (('TextArea',))
+               230 IMPORT_NAME             37 (components.text_area)
+               232 IMPORT_FROM             38 (TextArea)
+               234 STORE_NAME              38 (TextArea)
+               236 POP_TOP
+               238 PRECALL                 22
    consts
-      ('Anchor', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea')
+      ('Anchor', 'Badge', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea')
       2
       ('Anchor',)
       1
+      ('Badge',)
       ('Breadcrumb',)
       ('Button',)
       ('Checkbox',)
       ('Form',)
       ('FormItem',)
       ('Input',)
       ('Message',)
@@ -167,17 +176,17 @@
       ('Select',)
       ('Spin',)
       ('Switch',)
       ('Tab',)
       ('Table',)
       ('TextArea',)
       None
-   names      ('__all__', 'components.anchor', 'Anchor', 'components.breadcrumb', 'Breadcrumb', 'components.button', 'Button', 'components.checkbox', 'Checkbox', 'components.form', 'Form', 'components.form_item', 'FormItem', 'components.input', 'Input', 'components.message', 'Message', 'components.modal', 'Modal', 'components.page', 'Page', 'components.popover_confirm', 'PopoverConfirm', 'components.row', 'Row', 'components.select', 'Select', 'components.spin', 'Spin', 'components.switch', 'Switch', 'components.tab', 'Tab', 'components.table', 'Table', 'components.text_area', 'TextArea')
+   names      ('__all__', 'components.anchor', 'Anchor', 'components.badge', 'Badge', 'components.breadcrumb', 'Breadcrumb', 'components.button', 'Button', 'components.checkbox', 'Checkbox', 'components.form', 'Form', 'components.form_item', 'FormItem', 'components.input', 'Input', 'components.message', 'Message', 'components.modal', 'Modal', 'components.page', 'Page', 'components.popover_confirm', 'PopoverConfirm', 'components.row', 'Row', 'components.select', 'Select', 'components.spin', 'Spin', 'components.switch', 'Switch', 'components.tab', 'Tab', 'components.table', 'Table', 'components.text_area', 'TextArea')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/project/src/transstellar_antd/v4/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108150c010c010c010c010c010c010c010c010c010c010c010c
-      010c010c010c010c010c01
+      0x00ff020108160c010c010c010c010c010c010c010c010c010c010c010c
+      010c010c010c010c010c010c01
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/button.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/checkbox.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/checkbox.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/form_item.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/form_item.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/input.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/input.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/message.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/modal.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/modal.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/page.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/popover_confirm.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/popover_confirm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/row.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/row.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/select.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/select.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/switch.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/switch.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v4/components/__pycache__/table.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v4/components/__pycache__/table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/__init__.py` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __all__ = [
     "Anchor",
+    "Badge",
     "Breadcrumb",
     "Button",
     "Checkbox",
     "Form",
     "FormItem",
     "Input",
     "Message",
@@ -16,14 +17,15 @@
     "Switch",
     "Tab",
     "Table",
     "TextArea",
 ]
 
 from ..components.anchor import Anchor
+from .components.badge import Badge
 from .components.breadcrumb import Breadcrumb
 from .components.button import Button
 from .components.checkbox import Checkbox
 from .components.form import Form
 from .components.form_item import FormItem
 from .components.input import Input
 from .components.message import Message
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/__pycache__/__init__.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/__pycache__/__init__.cpython-312.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,162 +1,171 @@
 magic:    0xcb0d0d0a
-moddate:  0x680a4c66 (Tue May 21 02:43:52 2024 UTC)
-files sz: 967
+moddate:  0x7d025466 (Mon May 27 03:48:13 2024 UTC)
+files sz: 1016
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x970067006400a2015a00640164026c016d025a020100640364046c036d
       045a040100640364056c056d065a060100640364066c076d085a08010064
       0364076c096d0a5a0a0100640364086c0b6d0c5a0c0100640364096c0d6d
       0e5a0e01006403640a6c0f6d105a1001006403640b6c116d125a12010064
       03640c6c136d145a1401006403640d6c156d165a1601006403640e6c176d
       185a1801006403640f6c196d1a5a1a0100640364106c1b6d1c5a1c010064
       0364116c1d6d1e5a1e0100640364126c1f6d205a200100640364136c216d
-      225a220100640364146c236d245a240100a615
+      225a220100640364146c236d245a240100640364156c256d265a260100a6
+      16
      0           0 RESUME                   0
    
      1           2 BUILD_LIST               0
-                 4 LOAD_CONST               0 (('Anchor', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea'))
+                 4 LOAD_CONST               0 (('Anchor', 'Badge', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea'))
                  6 LIST_EXTEND              1
                  8 STORE_NAME               0 (__all__)
    
-    22          10 LOAD_CONST               1 (2)
+    23          10 LOAD_CONST               1 (2)
                 12 LOAD_CONST               2 (('Anchor',))
                 14 IMPORT_NAME              1 (components.anchor)
                 16 IMPORT_FROM              2 (Anchor)
                 18 STORE_NAME               2 (Anchor)
                 20 POP_TOP
    
-    23          22 LOAD_CONST               3 (1)
-                24 LOAD_CONST               4 (('Breadcrumb',))
-                26 IMPORT_NAME              3 (components.breadcrumb)
-                28 IMPORT_FROM              4 (Breadcrumb)
-                30 STORE_NAME               4 (Breadcrumb)
+    24          22 LOAD_CONST               3 (1)
+                24 LOAD_CONST               4 (('Badge',))
+                26 IMPORT_NAME              3 (components.badge)
+                28 IMPORT_FROM              4 (Badge)
+                30 STORE_NAME               4 (Badge)
                 32 POP_TOP
    
-    24          34 LOAD_CONST               3 (1)
-                36 LOAD_CONST               5 (('Button',))
-                38 IMPORT_NAME              5 (components.button)
-                40 IMPORT_FROM              6 (Button)
-                42 STORE_NAME               6 (Button)
+    25          34 LOAD_CONST               3 (1)
+                36 LOAD_CONST               5 (('Breadcrumb',))
+                38 IMPORT_NAME              5 (components.breadcrumb)
+                40 IMPORT_FROM              6 (Breadcrumb)
+                42 STORE_NAME               6 (Breadcrumb)
                 44 POP_TOP
    
-    25          46 LOAD_CONST               3 (1)
-                48 LOAD_CONST               6 (('Checkbox',))
-                50 IMPORT_NAME              7 (components.checkbox)
-                52 IMPORT_FROM              8 (Checkbox)
-                54 STORE_NAME               8 (Checkbox)
+    26          46 LOAD_CONST               3 (1)
+                48 LOAD_CONST               6 (('Button',))
+                50 IMPORT_NAME              7 (components.button)
+                52 IMPORT_FROM              8 (Button)
+                54 STORE_NAME               8 (Button)
                 56 POP_TOP
    
-    26          58 LOAD_CONST               3 (1)
-                60 LOAD_CONST               7 (('Form',))
-                62 IMPORT_NAME              9 (components.form)
-                64 IMPORT_FROM             10 (Form)
-                66 STORE_NAME              10 (Form)
+    27          58 LOAD_CONST               3 (1)
+                60 LOAD_CONST               7 (('Checkbox',))
+                62 IMPORT_NAME              9 (components.checkbox)
+                64 IMPORT_FROM             10 (Checkbox)
+                66 STORE_NAME              10 (Checkbox)
                 68 POP_TOP
    
-    27          70 LOAD_CONST               3 (1)
-                72 LOAD_CONST               8 (('FormItem',))
-                74 IMPORT_NAME             11 (components.form_item)
-                76 IMPORT_FROM             12 (FormItem)
-                78 STORE_NAME              12 (FormItem)
+    28          70 LOAD_CONST               3 (1)
+                72 LOAD_CONST               8 (('Form',))
+                74 IMPORT_NAME             11 (components.form)
+                76 IMPORT_FROM             12 (Form)
+                78 STORE_NAME              12 (Form)
                 80 POP_TOP
    
-    28          82 LOAD_CONST               3 (1)
-                84 LOAD_CONST               9 (('Input',))
-                86 IMPORT_NAME             13 (components.input)
-                88 IMPORT_FROM             14 (Input)
-                90 STORE_NAME              14 (Input)
+    29          82 LOAD_CONST               3 (1)
+                84 LOAD_CONST               9 (('FormItem',))
+                86 IMPORT_NAME             13 (components.form_item)
+                88 IMPORT_FROM             14 (FormItem)
+                90 STORE_NAME              14 (FormItem)
                 92 POP_TOP
    
-    29          94 LOAD_CONST               3 (1)
-                96 LOAD_CONST              10 (('Message',))
-                98 IMPORT_NAME             15 (components.message)
-               100 IMPORT_FROM             16 (Message)
-               102 STORE_NAME              16 (Message)
+    30          94 LOAD_CONST               3 (1)
+                96 LOAD_CONST              10 (('Input',))
+                98 IMPORT_NAME             15 (components.input)
+               100 IMPORT_FROM             16 (Input)
+               102 STORE_NAME              16 (Input)
                104 POP_TOP
    
-    30         106 LOAD_CONST               3 (1)
-               108 LOAD_CONST              11 (('Modal',))
-               110 IMPORT_NAME             17 (components.modal)
-               112 IMPORT_FROM             18 (Modal)
-               114 STORE_NAME              18 (Modal)
+    31         106 LOAD_CONST               3 (1)
+               108 LOAD_CONST              11 (('Message',))
+               110 IMPORT_NAME             17 (components.message)
+               112 IMPORT_FROM             18 (Message)
+               114 STORE_NAME              18 (Message)
                116 POP_TOP
    
-    31         118 LOAD_CONST               3 (1)
-               120 LOAD_CONST              12 (('Page',))
-               122 IMPORT_NAME             19 (components.page)
-               124 IMPORT_FROM             20 (Page)
-               126 STORE_NAME              20 (Page)
+    32         118 LOAD_CONST               3 (1)
+               120 LOAD_CONST              12 (('Modal',))
+               122 IMPORT_NAME             19 (components.modal)
+               124 IMPORT_FROM             20 (Modal)
+               126 STORE_NAME              20 (Modal)
                128 POP_TOP
    
-    32         130 LOAD_CONST               3 (1)
-               132 LOAD_CONST              13 (('PopoverConfirm',))
-               134 IMPORT_NAME             21 (components.popover_confirm)
-               136 IMPORT_FROM             22 (PopoverConfirm)
-               138 STORE_NAME              22 (PopoverConfirm)
+    33         130 LOAD_CONST               3 (1)
+               132 LOAD_CONST              13 (('Page',))
+               134 IMPORT_NAME             21 (components.page)
+               136 IMPORT_FROM             22 (Page)
+               138 STORE_NAME              22 (Page)
                140 POP_TOP
    
-    33         142 LOAD_CONST               3 (1)
-               144 LOAD_CONST              14 (('Row',))
-               146 IMPORT_NAME             23 (components.row)
-               148 IMPORT_FROM             24 (Row)
-               150 STORE_NAME              24 (Row)
+    34         142 LOAD_CONST               3 (1)
+               144 LOAD_CONST              14 (('PopoverConfirm',))
+               146 IMPORT_NAME             23 (components.popover_confirm)
+               148 IMPORT_FROM             24 (PopoverConfirm)
+               150 STORE_NAME              24 (PopoverConfirm)
                152 POP_TOP
    
-    34         154 LOAD_CONST               3 (1)
-               156 LOAD_CONST              15 (('Select',))
-               158 IMPORT_NAME             25 (components.select)
-               160 IMPORT_FROM             26 (Select)
-               162 STORE_NAME              26 (Select)
+    35         154 LOAD_CONST               3 (1)
+               156 LOAD_CONST              15 (('Row',))
+               158 IMPORT_NAME             25 (components.row)
+               160 IMPORT_FROM             26 (Row)
+               162 STORE_NAME              26 (Row)
                164 POP_TOP
    
-    35         166 LOAD_CONST               3 (1)
-               168 LOAD_CONST              16 (('Spin',))
-               170 IMPORT_NAME             27 (components.spin)
-               172 IMPORT_FROM             28 (Spin)
-               174 STORE_NAME              28 (Spin)
+    36         166 LOAD_CONST               3 (1)
+               168 LOAD_CONST              16 (('Select',))
+               170 IMPORT_NAME             27 (components.select)
+               172 IMPORT_FROM             28 (Select)
+               174 STORE_NAME              28 (Select)
                176 POP_TOP
    
-    36         178 LOAD_CONST               3 (1)
-               180 LOAD_CONST              17 (('Switch',))
-               182 IMPORT_NAME             29 (components.switch)
-               184 IMPORT_FROM             30 (Switch)
-               186 STORE_NAME              30 (Switch)
+    37         178 LOAD_CONST               3 (1)
+               180 LOAD_CONST              17 (('Spin',))
+               182 IMPORT_NAME             29 (components.spin)
+               184 IMPORT_FROM             30 (Spin)
+               186 STORE_NAME              30 (Spin)
                188 POP_TOP
    
-    37         190 LOAD_CONST               3 (1)
-               192 LOAD_CONST              18 (('Tab',))
-               194 IMPORT_NAME             31 (components.tab)
-               196 IMPORT_FROM             32 (Tab)
-               198 STORE_NAME              32 (Tab)
+    38         190 LOAD_CONST               3 (1)
+               192 LOAD_CONST              18 (('Switch',))
+               194 IMPORT_NAME             31 (components.switch)
+               196 IMPORT_FROM             32 (Switch)
+               198 STORE_NAME              32 (Switch)
                200 POP_TOP
    
-    38         202 LOAD_CONST               3 (1)
-               204 LOAD_CONST              19 (('Table',))
-               206 IMPORT_NAME             33 (components.table)
-               208 IMPORT_FROM             34 (Table)
-               210 STORE_NAME              34 (Table)
+    39         202 LOAD_CONST               3 (1)
+               204 LOAD_CONST              19 (('Tab',))
+               206 IMPORT_NAME             33 (components.tab)
+               208 IMPORT_FROM             34 (Tab)
+               210 STORE_NAME              34 (Tab)
                212 POP_TOP
    
-    39         214 LOAD_CONST               3 (1)
-               216 LOAD_CONST              20 (('TextArea',))
-               218 IMPORT_NAME             35 (components.text_area)
-               220 IMPORT_FROM             36 (TextArea)
-               222 STORE_NAME              36 (TextArea)
+    40         214 LOAD_CONST               3 (1)
+               216 LOAD_CONST              20 (('Table',))
+               218 IMPORT_NAME             35 (components.table)
+               220 IMPORT_FROM             36 (Table)
+               222 STORE_NAME              36 (Table)
                224 POP_TOP
-               226 PRECALL                 21
+   
+    41         226 LOAD_CONST               3 (1)
+               228 LOAD_CONST              21 (('TextArea',))
+               230 IMPORT_NAME             37 (components.text_area)
+               232 IMPORT_FROM             38 (TextArea)
+               234 STORE_NAME              38 (TextArea)
+               236 POP_TOP
+               238 PRECALL                 22
    consts
-      ('Anchor', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea')
+      ('Anchor', 'Badge', 'Breadcrumb', 'Button', 'Checkbox', 'Form', 'FormItem', 'Input', 'Message', 'Modal', 'Page', 'PopoverConfirm', 'Row', 'Select', 'Spin', 'Switch', 'Tab', 'Table', 'TextArea')
       2
       ('Anchor',)
       1
+      ('Badge',)
       ('Breadcrumb',)
       ('Button',)
       ('Checkbox',)
       ('Form',)
       ('FormItem',)
       ('Input',)
       ('Message',)
@@ -167,17 +176,17 @@
       ('Select',)
       ('Spin',)
       ('Switch',)
       ('Tab',)
       ('Table',)
       ('TextArea',)
       None
-   names      ('__all__', 'components.anchor', 'Anchor', 'components.breadcrumb', 'Breadcrumb', 'components.button', 'Button', 'components.checkbox', 'Checkbox', 'components.form', 'Form', 'components.form_item', 'FormItem', 'components.input', 'Input', 'components.message', 'Message', 'components.modal', 'Modal', 'components.page', 'Page', 'components.popover_confirm', 'PopoverConfirm', 'components.row', 'Row', 'components.select', 'Select', 'components.spin', 'Spin', 'components.switch', 'Switch', 'components.tab', 'Tab', 'components.table', 'Table', 'components.text_area', 'TextArea')
+   names      ('__all__', 'components.anchor', 'Anchor', 'components.badge', 'Badge', 'components.breadcrumb', 'Breadcrumb', 'components.button', 'Button', 'components.checkbox', 'Checkbox', 'components.form', 'Form', 'components.form_item', 'FormItem', 'components.input', 'Input', 'components.message', 'Message', 'components.modal', 'Modal', 'components.page', 'Page', 'components.popover_confirm', 'PopoverConfirm', 'components.row', 'Row', 'components.select', 'Select', 'components.spin', 'Spin', 'components.switch', 'Switch', 'components.tab', 'Tab', 'components.table', 'Table', 'components.text_area', 'TextArea')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/project/src/transstellar_antd/v5/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108150c010c010c010c010c010c010c010c010c010c010c010c
-      010c010c010c010c010c01
+      0x00ff020108160c010c010c010c010c010c010c010c010c010c010c010c
+      010c010c010c010c010c010c01
```

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/button.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/checkbox.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/checkbox.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form.cpython-312.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/form_item.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/form_item.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/input.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/input.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/message.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/modal.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/modal.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/page.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/page.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/popover_confirm.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/popover_confirm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/row.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/row.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/select.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/select.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/switch.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/switch.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `transstellar_antd-0.8.1/src/transstellar_antd/v5/components/__pycache__/table.cpython-38.pyc` & `transstellar_antd-0.9.0/src/transstellar_antd/v5/components/__pycache__/table.cpython-38.pyc`

 * *Files identical despite different names*

