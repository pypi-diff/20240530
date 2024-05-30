# Comparing `tmp/senderstats-1.2.2.tar.gz` & `tmp/senderstats-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senderstats-1.2.2.tar", last modified: Tue Apr 16 19:07:49 2024, max compression
+gzip compressed data, was "senderstats-1.2.3.tar", last modified: Thu May 30 18:26:52 2024, max compression
```

## Comparing `senderstats-1.2.2.tar` & `senderstats-1.2.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.400999 senderstats-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 19:07:43.000000 senderstats-1.2.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.393000 senderstats-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-16 19:07:43.000000 senderstats-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-16 19:07:43.000000 senderstats-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-16 19:07:49.396999 senderstats-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-04-16 19:07:43.000000 senderstats-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 19:07:43.000000 senderstats-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:07:49.400999 senderstats-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.393000 senderstats-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/lib/MessageDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/lib/MessageDataReport.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:43.000000 senderstats-1.2.2/src/senderstats/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:07:49.396999 senderstats-1.2.2/src/senderstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 19:07:49.000000 senderstats-1.2.2/src/senderstats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.046028 senderstats-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 18:26:47.000000 senderstats-1.2.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.042028 senderstats-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.042028 senderstats-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 18:26:47.000000 senderstats-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-30 18:26:47.000000 senderstats-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-30 18:26:52.046028 senderstats-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-30 18:26:47.000000 senderstats-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-30 18:26:47.000000 senderstats-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:26:52.046028 senderstats-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.042028 senderstats-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.046028 senderstats-1.2.3/src/senderstats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.046028 senderstats-1.2.3/src/senderstats/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.046028 senderstats-1.2.3/src/senderstats/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/lib/FieldMapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/lib/MessageDataProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12426 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/lib/MessageDataReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:47.000000 senderstats-1.2.3/src/senderstats/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:26:52.046028 senderstats-1.2.3/src/senderstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-30 18:26:52.000000 senderstats-1.2.3/src/senderstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-30 18:26:52.000000 senderstats-1.2.3/src/senderstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:26:52.000000 senderstats-1.2.3/src/senderstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 18:26:52.000000 senderstats-1.2.3/src/senderstats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 18:26:52.000000 senderstats-1.2.3/src/senderstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 18:26:52.000000 senderstats-1.2.3/src/senderstats.egg-info/top_level.txt
```

### Comparing `senderstats-1.2.2/.github/workflows/python-publish.yml` & `senderstats-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.2/.gitignore` & `senderstats-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.2/PKG-INFO` & `senderstats-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senderstats
-Version: 1.2.2
+Version: 1.2.3
 Summary: Tool to Process Smart Search Results and Identify Top Senders
 License: MIT
 Project-URL: repository, https://github.com/pfptcommunity/senderstats
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Requires-Dist: xlsxwriter
 Requires-Dist: tldextract
@@ -54,50 +54,65 @@
     * Total outbound messages
     * Total outbound average size
     * Total outbound peak hourly volume
 
 ### Usage Options:
 
 ```
-usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid]
-                   [-t N] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]]
-                   [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
+usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath]
+                   [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath]
+                   [--gen-alignment] [--gen-msgid] [-t N] [--no-display-name] [--remove-prvs] [--decode-srs]
+                   [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]]
+                   [--restrict-domains <domain> [<domain> ...]] [--excluded-senders <sender> [<sender> ...]]
+                   [--date-format DateFmt] [--show-skip-detail]
 
 This tool helps identify the top senders based on smart search outbound message exports.
 
-Required arguments (optional):
+Input / Output arguments (required):
   -i <file> [<file> ...], --input <file> [<file> ...]  Smart search files to read.
   -o <xlsx>, --output <xlsx>                           Output file
 
 Field mapping arguments (optional):
   --mfrom MFrom                                        CSV field of the envelope sender address. (default=Sender)
   --hfrom HFrom                                        CSV field of the header From: address. (default=Header_From)
-  --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-Path)
+  --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-
+                                                       Path)
   --msgid MsgID                                        CSV field of the message ID. (default=Message_ID)
-  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is specified. (default=Subject)
+  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is
+                                                       specified. (default=Subject)
   --size MsgSz                                         CSV field of message size. (default=Message_Size)
   --date Date                                          CSV field of message date/time. (default=Date)
 
 Reporting control arguments (optional):
-  --gen-hfrom                                          Generate report showing the header From: data for messages being sent.
+  --gen-hfrom                                          Generate report showing the header From: data for messages
+                                                       being sent.
   --gen-rpath                                          Generate report showing return path for messages being sent.
-  --gen-alignment                                      Generate report showing envelope sender and header From: alignment
-  --gen-msgid                                          Generate report showing parsed Message ID. Helps determine the sending system
-  -t N, --threshold N                                  Adjust summary report threshold for messages per day to be considered application traffic. (default=100)
+  --gen-alignment                                      Generate report showing envelope sender and header From:
+                                                       alignment
+  --gen-msgid                                          Generate report showing parsed Message ID. Helps determine the
+                                                       sending system
+  -t N, --threshold N                                  Adjust summary report threshold for messages per day to be
+                                                       considered application traffic. (default=100)
 
 Parsing behavior arguments (optional):
-  --no-display-name                                    Remove display and use address only. Converts 'Display Name <user@domain.com>' to 'user@domain.com'
-  --remove-prvs                                        Remove return path verification strings e.g. prvs=tag=sender@domain.com
-  --decode-srs                                         Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
-  --no-empty-hfrom                                     If the header From: is empty the envelope sender address is used
-  --sample-subject                                     Enable probabilistic random sampling of subject lines found during processing
+  --no-display-name                                    Remove display and use address only. Converts 'Display Name
+                                                       <user@domain.com>' to 'user@domain.com'
+  --remove-prvs                                        Remove return path verification strings e.g.
+                                                       prvs=tag=sender@domain.com
+  --decode-srs                                         Convert sender rewrite scheme,
+                                                       forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
+  --no-empty-hfrom                                     If the header From: is empty the envelope sender address is
+                                                       used
+  --sample-subject                                     Enable probabilistic random sampling of subject lines found
+                                                       during processing
   --excluded-domains <domain> [<domain> ...]           Exclude domains from processing.
   --restrict-domains <domain> [<domain> ...]           Constrain domains for processing.
   --excluded-senders <sender> [<sender> ...]           Exclude senders from processing.
-  --date-format DateFmt                                Date format used to parse the timestamps. (default=%Y-%m-%dT%H:%M:%S.%f%z)
+  --date-format DateFmt                                Date format used to parse the timestamps.
+                                                       (default=%Y-%m-%dT%H:%M:%S.%f%z)
 
 Extended processing controls (optional):
   --show-skip-detail                                   Show skipped details
 
 Usage:
   -h, --help                                           Show this help message and exit
 ```
```

### Comparing `senderstats-1.2.2/README.md` & `senderstats-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,50 +43,65 @@
     * Total outbound messages
     * Total outbound average size
     * Total outbound peak hourly volume
 
 ### Usage Options:
 
 ```
-usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid]
-                   [-t N] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]]
-                   [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
+usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath]
+                   [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath]
+                   [--gen-alignment] [--gen-msgid] [-t N] [--no-display-name] [--remove-prvs] [--decode-srs]
+                   [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]]
+                   [--restrict-domains <domain> [<domain> ...]] [--excluded-senders <sender> [<sender> ...]]
+                   [--date-format DateFmt] [--show-skip-detail]
 
 This tool helps identify the top senders based on smart search outbound message exports.
 
-Required arguments (optional):
+Input / Output arguments (required):
   -i <file> [<file> ...], --input <file> [<file> ...]  Smart search files to read.
   -o <xlsx>, --output <xlsx>                           Output file
 
 Field mapping arguments (optional):
   --mfrom MFrom                                        CSV field of the envelope sender address. (default=Sender)
   --hfrom HFrom                                        CSV field of the header From: address. (default=Header_From)
-  --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-Path)
+  --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-
+                                                       Path)
   --msgid MsgID                                        CSV field of the message ID. (default=Message_ID)
-  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is specified. (default=Subject)
+  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is
+                                                       specified. (default=Subject)
   --size MsgSz                                         CSV field of message size. (default=Message_Size)
   --date Date                                          CSV field of message date/time. (default=Date)
 
 Reporting control arguments (optional):
-  --gen-hfrom                                          Generate report showing the header From: data for messages being sent.
+  --gen-hfrom                                          Generate report showing the header From: data for messages
+                                                       being sent.
   --gen-rpath                                          Generate report showing return path for messages being sent.
-  --gen-alignment                                      Generate report showing envelope sender and header From: alignment
-  --gen-msgid                                          Generate report showing parsed Message ID. Helps determine the sending system
-  -t N, --threshold N                                  Adjust summary report threshold for messages per day to be considered application traffic. (default=100)
+  --gen-alignment                                      Generate report showing envelope sender and header From:
+                                                       alignment
+  --gen-msgid                                          Generate report showing parsed Message ID. Helps determine the
+                                                       sending system
+  -t N, --threshold N                                  Adjust summary report threshold for messages per day to be
+                                                       considered application traffic. (default=100)
 
 Parsing behavior arguments (optional):
-  --no-display-name                                    Remove display and use address only. Converts 'Display Name <user@domain.com>' to 'user@domain.com'
-  --remove-prvs                                        Remove return path verification strings e.g. prvs=tag=sender@domain.com
-  --decode-srs                                         Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
-  --no-empty-hfrom                                     If the header From: is empty the envelope sender address is used
-  --sample-subject                                     Enable probabilistic random sampling of subject lines found during processing
+  --no-display-name                                    Remove display and use address only. Converts 'Display Name
+                                                       <user@domain.com>' to 'user@domain.com'
+  --remove-prvs                                        Remove return path verification strings e.g.
+                                                       prvs=tag=sender@domain.com
+  --decode-srs                                         Convert sender rewrite scheme,
+                                                       forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
+  --no-empty-hfrom                                     If the header From: is empty the envelope sender address is
+                                                       used
+  --sample-subject                                     Enable probabilistic random sampling of subject lines found
+                                                       during processing
   --excluded-domains <domain> [<domain> ...]           Exclude domains from processing.
   --restrict-domains <domain> [<domain> ...]           Constrain domains for processing.
   --excluded-senders <sender> [<sender> ...]           Exclude senders from processing.
-  --date-format DateFmt                                Date format used to parse the timestamps. (default=%Y-%m-%dT%H:%M:%S.%f%z)
+  --date-format DateFmt                                Date format used to parse the timestamps.
+                                                       (default=%Y-%m-%dT%H:%M:%S.%f%z)
 
 Extended processing controls (optional):
   --show-skip-detail                                   Show skipped details
 
 Usage:
   -h, --help                                           Show this help message and exit
 ```
```

### Comparing `senderstats-1.2.2/src/senderstats/cli.py` & `senderstats-1.2.3/src/senderstats/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from glob import glob
 
 from senderstats.common.constants import DEFAULT_THRESHOLD, DEFAULT_DOMAIN_EXCLUSIONS
 from senderstats.common.utils import *
 from senderstats.common.validators import *
 from senderstats.lib.MessageDataProcessor import *
 from senderstats.lib.MessageDataReport import MessageDataReport
-
+from senderstats.lib.FieldMapper import *
 
 def parse_arguments():
     parser = argparse.ArgumentParser(prog="senderstats", add_help=False,
                                      description="""This tool helps identify the top senders based on smart search outbound message exports.""",
                                      formatter_class=lambda prog: argparse.HelpFormatter(prog, max_help_position=80))
 
-    required_group = parser.add_argument_group('Required arguments (optional)')
+    required_group = parser.add_argument_group('Input / Output arguments (required)')
     field_group = parser.add_argument_group('Field mapping arguments (optional)')
     reporting_group = parser.add_argument_group('Reporting control arguments (optional)')
     parser_group = parser.add_argument_group('Parsing behavior arguments (optional)')
     output_group = parser.add_argument_group('Extended processing controls (optional)')
     usage = parser.add_argument_group('Usage')
     # Manually add the help option to the new group
     usage.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS,
@@ -139,38 +139,40 @@
     args.restricted_domains = sorted(list({domain.casefold() for domain in args.restricted_domains}))
 
     print_list_with_title("Files to be processed:", file_names)
     print_list_with_title("Senders excluded from processing:", args.excluded_senders)
     print_list_with_title("Domains excluded from processing:", args.excluded_domains)
     print_list_with_title("Domains constrained or processing:", args.restricted_domains)
 
-    # Log processor object (find a cleaner way to apply these settings)
-    data_processor = MessageDataProcessor(args.excluded_senders, args.excluded_domains, args.restricted_domains)
-
     # Configure fields
-    if args.hfrom_field:
-        data_processor.set_hfrom_field(args.hfrom_field)
-
+    field_mapper = FieldMapper()
     if args.mfrom_field:
-        data_processor.set_hfrom_field(args.mfrom_field)
+        field_mapper.add_mapping('mfrom', args.mfrom_field)
+
+    if args.hfrom_field:
+        field_mapper.add_mapping('hfrom',args.hfrom_field)
 
     if args.rpath_field:
-        data_processor.set_rpath_field(args.rpath_field)
+        field_mapper.add_mapping('rpath', args.rpath_field)
 
     if args.msgid_field:
-        data_processor.set_msgid_field(args.msgid_field)
+        field_mapper.add_mapping('msgid', args.msgid_field)
 
     if args.msgsz_field:
-        data_processor.set_msgsz_field(args.msgsz_field)
+        field_mapper.add_mapping('msgsz', args.msgsz_field)
 
     if args.subject_field:
-        data_processor.set_subject_field(args.subject_field)
+        field_mapper.add_mapping('subject', args.subject_field)
 
     if args.date_field:
-        data_processor.set_date_field(args.date_field)
+        field_mapper.add_mapping('date', args.date_field)
+
+    # Log processor object (find a cleaner way to apply these settings)
+    data_processor = MessageDataProcessor(field_mapper, args.excluded_senders, args.excluded_domains, args.restricted_domains)
+
 
     if args.date_format:
         data_processor.set_date_format = args.date_format
 
     # Set processing flags
     if args.remove_prvs:
         data_processor.set_opt_remove_prvs(args.remove_prvs)
```

### Comparing `senderstats-1.2.2/src/senderstats/common/constants.py` & `senderstats-1.2.3/src/senderstats/common/constants.py`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.2/src/senderstats/common/utils.py` & `senderstats-1.2.3/src/senderstats/common/utils.py`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.2/src/senderstats/common/validators.py` & `senderstats-1.2.3/src/senderstats/common/validators.py`

 * *Files identical despite different names*

### Comparing `senderstats-1.2.2/src/senderstats/lib/MessageDataProcessor.py` & `senderstats-1.2.3/src/senderstats/lib/MessageDataProcessor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import csv
 import datetime
 import re
 from collections import defaultdict
 from random import random
 from typing import DefaultDict, Any, Dict, Set, List, Optional
-
 from tldextract import tldextract
-
 from senderstats.common.utils import (convert_srs, remove_prvs, compile_domains_pattern, find_ip_in_text,
                                       parse_email_details)
+from .FieldMapper import FieldMapper
 
-# Constants for the class
-DEFAULT_MFROM_FIELD = 'Sender'
-DEFAULT_HFROM_FIELD = 'Header_From'
-DEFAULT_RPATH_FIELD = 'Header_Return-Path'
-DEFAULT_MSGID_FIELD = 'Message_ID'
-DEFAULT_MSGSZ_FIELD = 'Message_Size'
-DEFAULT_SUBJECT_FIELD = 'Subject'
-DEFAULT_DATE_FIELD = 'Date'
 DEFAULT_DATE_FORMAT = '%Y-%m-%dT%H:%M:%S.%f%z'
 
 
 class MessageDataProcessor:
     # Data processing information
     __mfrom_data: Dict[str, Dict]
     __hfrom_data: Dict[str, Dict]
@@ -33,21 +24,15 @@
     __date_counter: DefaultDict[str, int]
     __total_processed_count: int
     __empty_sender_count: int
     __excluded_sender_count: DefaultDict[str, int]
     __excluded_domain_count: DefaultDict[str, int]
     __restricted_domains_count: DefaultDict[str, int]
     # Define CSV Fields
-    __mfrom_field: str
-    __hfrom_field: str
-    __rpath_field: str
-    __msgid_field: str
-    __msgsz_field: str
-    __subject_field: str
-    __date_field: str
+    __field_mapper: FieldMapper
     __date_format: str
     # Processing Option Flags
     __opt_no_display: bool
     __opt_decode_srs: bool
     __opt_remove_prvs: bool
     __opt_empty_from: bool
     __opt_sample_subject: bool
@@ -57,23 +42,18 @@
     __opt_gen_rpath: bool
     __opt_gen_msgid: bool
     # Restrictions
     __excluded_senders: Set[str]
     __excluded_domains: re.Pattern
     __restricted_domains: re.Pattern
 
-    def __init__(self, excluded_senders: List[str], excluded_domains: List[str], restricted_domains: List[str]):
+    def __init__(self, field_mapper: FieldMapper, excluded_senders: List[str], excluded_domains: List[str],
+                 restricted_domains: List[str]):
         # Default field mappings based on smart search output
-        self.__mfrom_field = DEFAULT_MFROM_FIELD
-        self.__hfrom_field = DEFAULT_HFROM_FIELD
-        self.__rpath_field = DEFAULT_RPATH_FIELD
-        self.__msgid_field = DEFAULT_MSGID_FIELD
-        self.__msgsz_field = DEFAULT_MSGSZ_FIELD
-        self.__subject_field = DEFAULT_SUBJECT_FIELD
-        self.__date_field = DEFAULT_DATE_FIELD
+        self.__field_mapper = field_mapper
         self.__date_format = DEFAULT_DATE_FORMAT
         # Initialize counters
         self.__date_counter = defaultdict(int)
         self.__total_processed_count = 0
         self.__empty_sender_count = 0
         self.__excluded_sender_count = defaultdict(int)
         self.__excluded_domain_count = defaultdict(int)
@@ -156,15 +136,15 @@
             rpath = remove_prvs(rpath)
 
         if self.__opt_decode_srs:
             rpath = convert_srs(rpath)
 
         return rpath
 
-    def __process_alignment_data(self, hfrom: str, mfrom: str, message_size: int, subject: Optional):
+    def __process_alignment_data(self, hfrom: str, mfrom: str, message_size: int, subject: str):
         # Fat index for binding commonality
         sender_header_index = (mfrom, hfrom)
         self.__mfrom_hfrom_data.setdefault(sender_header_index, {})
         self.__update_message_size_and_subjects(self.__mfrom_hfrom_data[sender_header_index], message_size, subject)
 
     def __process_msgid_data(self, msgid: str, mfrom: str, message_size: int, subject: str) -> str:
         # Message ID is unique but often the sending host behind the @ symbol is unique to the application
@@ -213,67 +193,75 @@
 
         # Ensure at least one subject is added if subjects array is empty
         if not data['subjects'] or random() < probability:
             data['subjects'].append(subject)
 
     def process_file(self, input_file):
         with (open(input_file, 'r', encoding='utf-8-sig') as input_file):
-            reader = csv.DictReader(input_file)
+            reader = csv.reader(input_file)
+            headers = next(reader)  # Read the first line which contains the headers
+            self.__field_mapper.configure(headers)
             for csv_line in reader:
                 self.__total_processed_count += 1
 
                 # Make sure cast to int is valid, else 0 (size is required)
-                message_size = csv_line[self.__msgsz_field]
+                message_size = self.__field_mapper.get_field(csv_line, 'msgsz')
+
                 if message_size.isdigit():
                     message_size = int(message_size)
                 else:
                     message_size = 0
 
-                mfrom = self.__process_mfrom_data(csv_line[self.__mfrom_field].casefold().strip())
+                mfrom = self.__field_mapper.get_field(csv_line, 'mfrom').casefold().strip()
+                mfrom = self.__process_mfrom_data(mfrom)
 
                 # mfrom will be None, unless the filtering criteria applied properly
                 if not mfrom:
                     continue
 
                 subject = ''
+                # Not all CSV files will contain a subject field.
                 if self.__opt_sample_subject:
-                    subject = csv_line[self.__subject_field].strip()
+                    subject = self.__field_mapper.get_field(csv_line, 'subject').casefold().strip()
 
                 # Track the cleaned, filtered mfrom data for our report
                 self.__mfrom_data.setdefault(mfrom, {})
                 self.__update_message_size_and_subjects(self.__mfrom_data[mfrom], message_size, subject)
 
                 # Alignment will require that we have hfrom
                 if self.__opt_gen_hfrom or self.__opt_gen_alignment:
-                    hfrom = self.__process_hfrom_data(csv_line[self.__hfrom_field].casefold().strip(), mfrom)
+                    hfrom = self.__field_mapper.get_field(csv_line, 'hfrom').casefold().strip()
+                    hfrom = self.__process_hfrom_data(hfrom, mfrom)
 
                     # Generate data for HFrom
                     if self.__opt_gen_hfrom:
                         self.__hfrom_data.setdefault(hfrom, {})
                         self.__update_message_size_and_subjects(self.__hfrom_data[hfrom], message_size, subject)
 
                     # Generate data for HFrom and MFrom Alignment
                     if self.__opt_gen_alignment:
                         self.__process_alignment_data(hfrom, mfrom, message_size, subject)
 
                 # Generate data for return path
                 if self.__opt_gen_rpath:
-                    rpath = self.__process_rpath_data(csv_line[self.__rpath_field].casefold().strip())
+                    rpath = self.__field_mapper.get_field(csv_line, 'rpath').casefold().strip()
+                    rpath = self.__process_rpath_data(rpath)
                     if self.__opt_gen_rpath:
                         self.__rpath_data.setdefault(rpath, {})
                         self.__update_message_size_and_subjects(self.__rpath_data[rpath], message_size, subject)
 
                 # Generate data for parsed message ID
                 if self.__opt_gen_msgid:
                     # Generate data for Message ID information
-                    self.__process_msgid_data(csv_line[self.__msgid_field].casefold().strip('<>[] '), mfrom,
-                                              message_size, subject)
+                    msgid = self.__field_mapper.get_field(csv_line, 'msgid').casefold().strip('<>[] ')
+                    self.__process_msgid_data(msgid, mfrom, message_size, subject)
 
                 # Determine distinct dates of data, and count number of messages on that day
-                date = datetime.datetime.strptime(csv_line[self.__date_field], self.__date_format)
+                date_str = self.__field_mapper.get_field(csv_line, 'date')
+                date = datetime.datetime.strptime(date_str, self.__date_format)
                 str_date = date.strftime('%Y-%m-%d')
                 self.__date_counter[str_date] += 1
 
     # Getter for total_processed_count
     def get_total_processed_count(self) -> int:
         return self.__total_processed_count
```

### Comparing `senderstats-1.2.2/src/senderstats/lib/MessageDataReport.py` & `senderstats-1.2.3/src/senderstats/lib/MessageDataReport.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,54 +103,54 @@
         summary.write(8, 0, "Total Outbound Data", self.__summary_format)
         summary.write(9, 0, "Total Messages Message", self.__summary_format)
         summary.write(10, 0, "Total Average Message Size", self.__summary_format)
         summary.write(11, 0, "Total Peak Hourly Volume", self.__summary_format)
 
         # Total summary of App data
         summary.write_formula(0, 1,
-                              "=IF(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)<1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)&\" bytes\",IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)>=1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)<POWER(1024,2)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/1024),1)&\" Kb\"),IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)>=POWER(1024,2),SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)<POWER(1024,3)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/POWER(1024,2)),1)&\" Mb\"),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/POWER(1024,3)),1)&\" Gb\"))))".format(
+                              "=IF(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)<1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)&\" B\",IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)>=1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)<POWER(1024,2)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/1024),1)&\" KB\"),IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)>=POWER(1024,2),SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)<POWER(1024,3)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/POWER(1024,2)),1)&\" MB\"),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/POWER(1024,3)),1)&\" GB\"))))".format(
                                   threshold=self.__threshold),
                               self.__summary_values_format)
 
         summary.write_formula(1, 1, "=SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!B:B)".format(
             threshold=self.__threshold),
                               self.__summary_values_format)
 
         summary.write_formula(2, 1,
-                              "=ROUNDUP((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!B:B))/1024,0)&\" Kb\"".format(
+                              "=ROUNDUP((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!B:B))/1024,0)&\" KB\"".format(
                                   threshold=self.__threshold),
                               self.__summary_values_format)
 
         summary.write_formula(3, 1,
                               "=ROUNDUP(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!B:B)/{days}/8,0)".format(
                                   days=self.__days,
                                   threshold=self.__threshold),
                               self.__summary_values_format)
 
         # 30 day calculation divide total days * 30
         summary.write_formula(5, 1,
-                              "=IF(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30<1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30&\" bytes\",IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30>=1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30<POWER(1024,2)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30/1024),1)&\" Kb\"),IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30>=POWER(1024,2),SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30<POWER(1024,3)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30/POWER(1024,2)),1)&\" Mb\"),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30/POWER(1024,3)),1)&\" Gb\"))))".format(
+                              "=IF(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30<1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30&\" B\",IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30>=1024,SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30<POWER(1024,2)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30/1024),1)&\" KB\"),IF(AND(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30>=POWER(1024,2),SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30<POWER(1024,3)),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30/POWER(1024,2)),1)&\" MB\"),(ROUND((SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!E:E)/{days}*30/POWER(1024,3)),1)&\" GB\"))))".format(
                                   days=self.__days,
                                   threshold=self.__threshold),
                               self.__summary_values_format)
 
         summary.write_formula(6, 1,
                               "=ROUNDUP(SUMIF('Envelope Senders'!D:D,\">={threshold}\",'Envelope Senders'!B:B)/{days}*30,0)".format(
                                   days=self.__days,
                                   threshold=self.__threshold),
                               self.__summary_values_format)
 
         # Total message volume data
         summary.write_formula(8, 1,
-                              "=IF(SUM('Envelope Senders'!E:E)<1024,SUM('Envelope Senders'!E:E)&\" bytes\",IF(AND(SUM('Envelope Senders'!E:E)>=1024,SUM('Envelope Senders'!E:E)<POWER(1024,2)),(ROUND((SUM('Envelope Senders'!E:E)/1024),1)&\" Kb\"),IF(AND(SUM('Envelope Senders'!E:E)>=POWER(1024,2),SUM('Envelope Senders'!E:E)<POWER(1024,3)),(ROUND((SUM('Envelope Senders'!E:E)/POWER(1024,2)),1)&\" Mb\"),(ROUND((SUM('Envelope Senders'!E:E)/POWER(1024,3)),1)&\" Gb\"))))",
+                              "=IF(SUM('Envelope Senders'!E:E)<1024,SUM('Envelope Senders'!E:E)&\" B\",IF(AND(SUM('Envelope Senders'!E:E)>=1024,SUM('Envelope Senders'!E:E)<POWER(1024,2)),(ROUND((SUM('Envelope Senders'!E:E)/1024),1)&\" KB\"),IF(AND(SUM('Envelope Senders'!E:E)>=POWER(1024,2),SUM('Envelope Senders'!E:E)<POWER(1024,3)),(ROUND((SUM('Envelope Senders'!E:E)/POWER(1024,2)),1)&\" MB\"),(ROUND((SUM('Envelope Senders'!E:E)/POWER(1024,3)),1)&\" GB\"))))",
                               self.__summary_values_format)
         summary.write_formula(9, 1, "=SUM('Envelope Senders'!B:B)", self.__summary_values_format)
 
         summary.write_formula(10, 1,
-                              "=ROUNDUP((SUM('Envelope Senders'!E:E)/SUM('Envelope Senders'!B:B))/1024,0)&\" Kb\"".format(
+                              "=ROUNDUP((SUM('Envelope Senders'!E:E)/SUM('Envelope Senders'!B:B))/1024,0)&\" KB\"".format(
                                   threshold=self.__threshold),
                               self.__summary_values_format)
 
         summary.write_formula(11, 1,
                               "=ROUNDUP(SUM('Envelope Senders'!B:B)/{days}/8,0)".format(
                                   days=self.__days,
                                   threshold=self.__threshold),
```

### Comparing `senderstats-1.2.2/src/senderstats.egg-info/PKG-INFO` & `senderstats-1.2.3/src/senderstats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senderstats
-Version: 1.2.2
+Version: 1.2.3
 Summary: Tool to Process Smart Search Results and Identify Top Senders
 License: MIT
 Project-URL: repository, https://github.com/pfptcommunity/senderstats
 Requires-Python: >3.9
 Description-Content-Type: text/markdown
 Requires-Dist: xlsxwriter
 Requires-Dist: tldextract
@@ -54,50 +54,65 @@
     * Total outbound messages
     * Total outbound average size
     * Total outbound peak hourly volume
 
 ### Usage Options:
 
 ```
-usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath] [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath] [--gen-alignment] [--gen-msgid]
-                   [-t N] [--no-display-name] [--remove-prvs] [--decode-srs] [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]] [--restrict-domains <domain> [<domain> ...]]
-                   [--excluded-senders <sender> [<sender> ...]] [--date-format DateFmt] [--show-skip-detail]
+usage: senderstats [-h] -i <file> [<file> ...] -o <xlsx> [--mfrom MFrom] [--hfrom HFrom] [--rpath RPath]
+                   [--msgid MsgID] [--subject Subject] [--size MsgSz] [--date Date] [--gen-hfrom] [--gen-rpath]
+                   [--gen-alignment] [--gen-msgid] [-t N] [--no-display-name] [--remove-prvs] [--decode-srs]
+                   [--no-empty-hfrom] [--sample-subject] [--excluded-domains <domain> [<domain> ...]]
+                   [--restrict-domains <domain> [<domain> ...]] [--excluded-senders <sender> [<sender> ...]]
+                   [--date-format DateFmt] [--show-skip-detail]
 
 This tool helps identify the top senders based on smart search outbound message exports.
 
-Required arguments (optional):
+Input / Output arguments (required):
   -i <file> [<file> ...], --input <file> [<file> ...]  Smart search files to read.
   -o <xlsx>, --output <xlsx>                           Output file
 
 Field mapping arguments (optional):
   --mfrom MFrom                                        CSV field of the envelope sender address. (default=Sender)
   --hfrom HFrom                                        CSV field of the header From: address. (default=Header_From)
-  --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-Path)
+  --rpath RPath                                        CSV field of the Return-Path: address. (default=Header_Return-
+                                                       Path)
   --msgid MsgID                                        CSV field of the message ID. (default=Message_ID)
-  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is specified. (default=Subject)
+  --subject Subject                                    CSV field of the Subject, only used if --sample-subject is
+                                                       specified. (default=Subject)
   --size MsgSz                                         CSV field of message size. (default=Message_Size)
   --date Date                                          CSV field of message date/time. (default=Date)
 
 Reporting control arguments (optional):
-  --gen-hfrom                                          Generate report showing the header From: data for messages being sent.
+  --gen-hfrom                                          Generate report showing the header From: data for messages
+                                                       being sent.
   --gen-rpath                                          Generate report showing return path for messages being sent.
-  --gen-alignment                                      Generate report showing envelope sender and header From: alignment
-  --gen-msgid                                          Generate report showing parsed Message ID. Helps determine the sending system
-  -t N, --threshold N                                  Adjust summary report threshold for messages per day to be considered application traffic. (default=100)
+  --gen-alignment                                      Generate report showing envelope sender and header From:
+                                                       alignment
+  --gen-msgid                                          Generate report showing parsed Message ID. Helps determine the
+                                                       sending system
+  -t N, --threshold N                                  Adjust summary report threshold for messages per day to be
+                                                       considered application traffic. (default=100)
 
 Parsing behavior arguments (optional):
-  --no-display-name                                    Remove display and use address only. Converts 'Display Name <user@domain.com>' to 'user@domain.com'
-  --remove-prvs                                        Remove return path verification strings e.g. prvs=tag=sender@domain.com
-  --decode-srs                                         Convert sender rewrite scheme, forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
-  --no-empty-hfrom                                     If the header From: is empty the envelope sender address is used
-  --sample-subject                                     Enable probabilistic random sampling of subject lines found during processing
+  --no-display-name                                    Remove display and use address only. Converts 'Display Name
+                                                       <user@domain.com>' to 'user@domain.com'
+  --remove-prvs                                        Remove return path verification strings e.g.
+                                                       prvs=tag=sender@domain.com
+  --decode-srs                                         Convert sender rewrite scheme,
+                                                       forwardmailbox+srs=hash=tt=domain.com=user to user@domain.com
+  --no-empty-hfrom                                     If the header From: is empty the envelope sender address is
+                                                       used
+  --sample-subject                                     Enable probabilistic random sampling of subject lines found
+                                                       during processing
   --excluded-domains <domain> [<domain> ...]           Exclude domains from processing.
   --restrict-domains <domain> [<domain> ...]           Constrain domains for processing.
   --excluded-senders <sender> [<sender> ...]           Exclude senders from processing.
-  --date-format DateFmt                                Date format used to parse the timestamps. (default=%Y-%m-%dT%H:%M:%S.%f%z)
+  --date-format DateFmt                                Date format used to parse the timestamps.
+                                                       (default=%Y-%m-%dT%H:%M:%S.%f%z)
 
 Extended processing controls (optional):
   --show-skip-detail                                   Show skipped details
 
 Usage:
   -h, --help                                           Show this help message and exit
 ```
```

### Comparing `senderstats-1.2.2/src/senderstats.egg-info/SOURCES.txt` & `senderstats-1.2.3/src/senderstats.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 src/senderstats.egg-info/entry_points.txt
 src/senderstats.egg-info/requires.txt
 src/senderstats.egg-info/top_level.txt
 src/senderstats/common/__init__.py
 src/senderstats/common/constants.py
 src/senderstats/common/utils.py
 src/senderstats/common/validators.py
+src/senderstats/lib/FieldMapper.py
 src/senderstats/lib/MessageDataProcessor.py
 src/senderstats/lib/MessageDataReport.py
 src/senderstats/lib/__init__.py
```

