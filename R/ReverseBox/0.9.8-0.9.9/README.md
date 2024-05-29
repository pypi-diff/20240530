# Comparing `tmp/ReverseBox-0.9.8.tar.gz` & `tmp/ReverseBox-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.9.8.tar", last modified: Sun May 12 13:09:13 2024, max compression
+gzip compressed data, was "ReverseBox-0.9.9.tar", last modified: Fri May 24 09:01:42 2024, max compression
```

## Comparing `ReverseBox-0.9.8.tar` & `ReverseBox-0.9.9.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.960686 ReverseBox-0.9.8/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.9.8/LICENSE
--rw-rw-rw-   0        0        0     7199 2024-05-12 13:09:13.960686 ReverseBox-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     5798 2024-05-12 13:07:54.000000 ReverseBox-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.898852 ReverseBox-0.9.8/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     7199 2024-05-12 13:09:13.000000 ReverseBox-0.9.8/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2024-05-12 13:09:13.000000 ReverseBox-0.9.8/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 13:09:13.000000 ReverseBox-0.9.8/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-12 13:09:13.000000 ReverseBox-0.9.8/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 13:09:13.000000 ReverseBox-0.9.8/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.899849 ReverseBox-0.9.8/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.9.8/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.905833 ReverseBox-0.9.8/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.8/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.9.8/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.9.8/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.9.8/reversebox/checksum/checksum_fletcher32.py
--rw-rw-rw-   0        0        0      339 2024-05-10 15:23:32.000000 ReverseBox-0.9.8/reversebox/checksum/checksum_sum8.py
--rw-rw-rw-   0        0        0      420 2024-05-10 14:15:25.000000 ReverseBox-0.9.8/reversebox/checksum/checksum_unix_sum_bsd16.py
--rw-rw-rw-   0        0        0      543 2024-05-10 15:23:32.000000 ReverseBox-0.9.8/reversebox/checksum/checksum_unix_sum_sysv.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.908825 ReverseBox-0.9.8/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.9.8/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.9.8/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.9.8/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.913812 ReverseBox-0.9.8/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.8/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.9.8/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.9.8/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0     2188 2024-05-06 16:03:40.000000 ReverseBox-0.9.8/reversebox/compression/compression_refpack.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.9.8/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.924782 ReverseBox-0.9.8/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.9.8/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.9.8/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.9.8/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.9.8/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.9.8/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.9.8/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.9.8/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.9.8/reversebox/crc/crc32_asobo.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.9.8/reversebox/crc/crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.9.8/reversebox/crc/crc64_asobo.py
--rw-rw-rw-   0        0        0      607 2024-05-12 13:08:50.000000 ReverseBox-0.9.8/reversebox/crc/crc64_go_iso.py
--rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.9.8/reversebox/crc/crc8.py
--rw-rw-rw-   0        0        0     5094 2024-05-12 00:00:36.000000 ReverseBox-0.9.8/reversebox/crc/crc_unix_cksum.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.929769 ReverseBox-0.9.8/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.8/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.9.8/reversebox/encryption/encryption_rot13.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.9.8/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.9.8/reversebox/encryption/encryption_xor_basic_key_guesser.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.9.8/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.9.8/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.934755 ReverseBox-0.9.8/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.8/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.9.8/reversebox/hash/hash_fnv.py
--rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.9.8/reversebox/hash/hash_md2.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.9.8/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.9.8/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.9.8/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.939742 ReverseBox-0.9.8/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.9.8/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.9.8/reversebox/image/image_dds.py
--rw-rw-rw-   0        0        0    12952 2024-05-06 14:14:06.000000 ReverseBox-0.9.8/reversebox/image/image_decoder.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.9.8/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.9.8/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0      668 2024-05-06 14:13:59.000000 ReverseBox-0.9.8/reversebox/image/image_formats.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.947721 ReverseBox-0.9.8/reversebox/image/swizzling/
--rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.9.8/reversebox/image/swizzling/__init__.py
--rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_3ds.py
--rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_cmpr.py
--rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_ps2.py
--rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_psp.py
--rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_psvita.py
--rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_switch.py
--rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_xbox.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.953705 ReverseBox-0.9.8/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.8/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.9.8/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 13:01:53.000000 ReverseBox-0.9.8/reversebox/io_files/bytes_helper_functions.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.9.8/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.9.8/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.9.8/reversebox/io_files/mod_handler.py
--rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.9.8/reversebox/io_files/translation_text_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:09:13.954702 ReverseBox-0.9.8/reversebox/libs/
--rw-rw-rw-   0        0        0        0 2024-05-03 23:15:20.000000 ReverseBox-0.9.8/reversebox/libs/__init__.py
--rw-rw-rw-   0        0        0  2557648 2024-05-03 19:25:24.000000 ReverseBox-0.9.8/reversebox/libs/refpack.dll
--rw-rw-rw-   0        0        0       42 2024-05-12 13:09:13.960686 ReverseBox-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1984 2024-05-12 13:08:45.000000 ReverseBox-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.219748 ReverseBox-0.9.9/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0     7247 2024-05-24 09:01:42.218751 ReverseBox-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5846 2024-05-24 08:58:59.000000 ReverseBox-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.153924 ReverseBox-0.9.9/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     7247 2024-05-24 09:01:42.000000 ReverseBox-0.9.9/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2602 2024-05-24 09:01:42.000000 ReverseBox-0.9.9/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:01:42.000000 ReverseBox-0.9.9/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-24 09:01:42.000000 ReverseBox-0.9.9/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 09:01:42.000000 ReverseBox-0.9.9/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.154921 ReverseBox-0.9.9/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.9.9/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.162900 ReverseBox-0.9.9/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.9/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_fletcher32.py
+-rw-rw-rw-   0        0        0      339 2024-05-10 15:23:32.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_sum8.py
+-rw-rw-rw-   0        0        0      375 2024-05-24 08:48:43.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_sum8_2s_complement.py
+-rw-rw-rw-   0        0        0      420 2024-05-10 14:15:25.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_unix_sum_bsd16.py
+-rw-rw-rw-   0        0        0      543 2024-05-10 15:23:32.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_unix_sum_sysv.py
+-rw-rw-rw-   0        0        0      339 2024-05-24 08:33:09.000000 ReverseBox-0.9.9/reversebox/checksum/checksum_xor8.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.164894 ReverseBox-0.9.9/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.9.9/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.9.9/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.9.9/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.169881 ReverseBox-0.9.9/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.9/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-03 14:40:28.000000 ReverseBox-0.9.9/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.9.9/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0     2188 2024-05-06 16:03:40.000000 ReverseBox-0.9.9/reversebox/compression/compression_refpack.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.9.9/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.182846 ReverseBox-0.9.9/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.9.9/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.9.9/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.9.9/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.9.9/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.9.9/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.9.9/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.9.9/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.9.9/reversebox/crc/crc32_asobo.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.9.9/reversebox/crc/crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.9.9/reversebox/crc/crc64_asobo.py
+-rw-rw-rw-   0        0        0      607 2024-05-12 13:08:50.000000 ReverseBox-0.9.9/reversebox/crc/crc64_go_iso.py
+-rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.9.9/reversebox/crc/crc8.py
+-rw-rw-rw-   0        0        0     5094 2024-05-12 00:00:36.000000 ReverseBox-0.9.9/reversebox/crc/crc_unix_cksum.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.187833 ReverseBox-0.9.9/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.9/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.9.9/reversebox/encryption/encryption_rot13.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.9.9/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.9.9/reversebox/encryption/encryption_xor_basic_key_guesser.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.9.9/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.9.9/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.193817 ReverseBox-0.9.9/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.9/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.9.9/reversebox/hash/hash_fnv.py
+-rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.9.9/reversebox/hash/hash_md2.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.9.9/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.9.9/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.9.9/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.198804 ReverseBox-0.9.9/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.9.9/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.9.9/reversebox/image/image_dds.py
+-rw-rw-rw-   0        0        0    12952 2024-05-06 14:14:06.000000 ReverseBox-0.9.9/reversebox/image/image_decoder.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.9.9/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.9.9/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0      668 2024-05-06 14:13:59.000000 ReverseBox-0.9.9/reversebox/image/image_formats.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.205785 ReverseBox-0.9.9/reversebox/image/swizzling/
+-rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.9.9/reversebox/image/swizzling/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_3ds.py
+-rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_cmpr.py
+-rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_ps2.py
+-rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_psp.py
+-rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_psvita.py
+-rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_switch.py
+-rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_xbox.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.212766 ReverseBox-0.9.9/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.9.9/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.9.9/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 13:01:53.000000 ReverseBox-0.9.9/reversebox/io_files/bytes_helper_functions.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.9.9/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.9.9/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.9.9/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.9.9/reversebox/io_files/translation_text_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:01:42.214761 ReverseBox-0.9.9/reversebox/libs/
+-rw-rw-rw-   0        0        0        0 2024-05-03 23:15:20.000000 ReverseBox-0.9.9/reversebox/libs/__init__.py
+-rw-rw-rw-   0        0        0  2557648 2024-05-03 19:25:24.000000 ReverseBox-0.9.9/reversebox/libs/refpack.dll
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:01:42.219748 ReverseBox-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-24 08:30:59.000000 ReverseBox-0.9.9/setup.py
```

### Comparing `ReverseBox-0.9.8/LICENSE` & `ReverseBox-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/PKG-INFO` & `ReverseBox-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.9.8
+Version: 0.9.9
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -56,16 +56,18 @@
 # List of functionalities
 
 * Checksum
   - Adler32 ✔️
   - Fletcher16 ✔️
   - Fletcher32 ✔️
   - Sum8 ✔️
+  - Sum8 2s Complement ✔️
   - Unix Sum BSD16 ✔️
   - Unix Sum SYSV ✔️
+  - Xor8 ✔️
 
 * CRC
   - CRC-8 ✔️
   - CRC-8/CDMA2000 ✔️
   - CRC-8/DARC ✔️ <span style="color:yellow">(wrapper only)</span>
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
```

### Comparing `ReverseBox-0.9.8/README.md` & `ReverseBox-0.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 # List of functionalities
 
 * Checksum
   - Adler32 ✔️
   - Fletcher16 ✔️
   - Fletcher32 ✔️
   - Sum8 ✔️
+  - Sum8 2s Complement ✔️
   - Unix Sum BSD16 ✔️
   - Unix Sum SYSV ✔️
+  - Xor8 ✔️
 
 * CRC
   - CRC-8 ✔️
   - CRC-8/CDMA2000 ✔️
   - CRC-8/DARC ✔️ <span style="color:yellow">(wrapper only)</span>
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
```

### Comparing `ReverseBox-0.9.8/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.9.9/ReverseBox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.9.8
+Version: 0.9.9
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python,image,decode,decoding,RGB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -56,16 +56,18 @@
 # List of functionalities
 
 * Checksum
   - Adler32 ✔️
   - Fletcher16 ✔️
   - Fletcher32 ✔️
   - Sum8 ✔️
+  - Sum8 2s Complement ✔️
   - Unix Sum BSD16 ✔️
   - Unix Sum SYSV ✔️
+  - Xor8 ✔️
 
 * CRC
   - CRC-8 ✔️
   - CRC-8/CDMA2000 ✔️
   - CRC-8/DARC ✔️ <span style="color:yellow">(wrapper only)</span>
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
```

### Comparing `ReverseBox-0.9.8/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.9.9/ReverseBox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 ReverseBox.egg-info/top_level.txt
 reversebox/__init__.py
 reversebox/checksum/__init__.py
 reversebox/checksum/checksum_adler32.py
 reversebox/checksum/checksum_fletcher16.py
 reversebox/checksum/checksum_fletcher32.py
 reversebox/checksum/checksum_sum8.py
+reversebox/checksum/checksum_sum8_2s_complement.py
 reversebox/checksum/checksum_unix_sum_bsd16.py
 reversebox/checksum/checksum_unix_sum_sysv.py
+reversebox/checksum/checksum_xor8.py
 reversebox/common/__init__.py
 reversebox/common/common.py
 reversebox/common/logger.py
 reversebox/compression/__init__.py
 reversebox/compression/compression_jcalg1.py
 reversebox/compression/compression_lzo.py
 reversebox/compression/compression_refpack.py
```

### Comparing `ReverseBox-0.9.8/reversebox/checksum/checksum_unix_sum_sysv.py` & `ReverseBox-0.9.9/reversebox/checksum/checksum_unix_sum_sysv.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/common/logger.py` & `ReverseBox-0.9.9/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/compression/compression_refpack.py` & `ReverseBox-0.9.9/reversebox/compression/compression_refpack.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc16_arc.py` & `ReverseBox-0.9.9/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.9.9/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.9.9/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.9.9/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.9.9/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc16_sick.py` & `ReverseBox-0.9.9/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc32_asobo.py` & `ReverseBox-0.9.9/reversebox/crc/crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.9.9/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc64_asobo.py` & `ReverseBox-0.9.9/reversebox/crc/crc64_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc64_go_iso.py` & `ReverseBox-0.9.9/reversebox/crc/crc64_go_iso.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc8.py` & `ReverseBox-0.9.9/reversebox/crc/crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/crc/crc_unix_cksum.py` & `ReverseBox-0.9.9/reversebox/crc/crc_unix_cksum.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/encryption/encryption_rot13.py` & `ReverseBox-0.9.9/reversebox/encryption/encryption_rot13.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.9.9/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/encryption/encryption_xor_basic_key_guesser.py` & `ReverseBox-0.9.9/reversebox/encryption/encryption_xor_basic_key_guesser.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.9.9/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.9.9/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/hash/hash_fnv.py` & `ReverseBox-0.9.9/reversebox/hash/hash_fnv.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/image_dds.py` & `ReverseBox-0.9.9/reversebox/image/image_dds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/image_decoder.py` & `ReverseBox-0.9.9/reversebox/image/image_decoder.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/image_finder_gui.py` & `ReverseBox-0.9.9/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/image_finder_main.py` & `ReverseBox-0.9.9/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/image_formats.py` & `ReverseBox-0.9.9/reversebox/image/image_formats.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_3ds.py` & `ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_3ds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_cmpr.py` & `ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_cmpr.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_ps2.py` & `ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_ps2.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_psp.py` & `ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_psp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_psvita.py` & `ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_psvita.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/image/swizzling/swizzle_switch.py` & `ReverseBox-0.9.9/reversebox/image/swizzling/swizzle_switch.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.9.9/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/io_files/bytes_helper_functions.py` & `ReverseBox-0.9.9/reversebox/io_files/bytes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/io_files/check_file.py` & `ReverseBox-0.9.9/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/io_files/file_handler.py` & `ReverseBox-0.9.9/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/io_files/mod_handler.py` & `ReverseBox-0.9.9/reversebox/io_files/mod_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.9.9/reversebox/io_files/translation_text_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/reversebox/libs/refpack.dll` & `ReverseBox-0.9.9/reversebox/libs/refpack.dll`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.9.8/setup.py` & `ReverseBox-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.9.8"
+VERSION_NUM = "0.9.9"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

