# Comparing `tmp/pan-chainguard-0.0.0.tar.gz` & `tmp/pan-chainguard-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan-chainguard-0.0.0.tar", last modified: Fri Mar 15 18:09:31 2024, max compression
+gzip compressed data, was "pan-chainguard-0.1.0.tar", last modified: Tue Apr  9 18:56:03 2024, max compression
```

## Comparing `pan-chainguard-0.0.0.tar` & `pan-chainguard-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-03-15 18:09:31.289784 pan-chainguard-0.0.0/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      883 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/LICENSE.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2707 2024-03-15 18:09:31.289784 pan-chainguard-0.0.0/PKG-INFO
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2172 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/README.rst
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-03-15 18:09:31.279784 pan-chainguard-0.0.0/bin/
--rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)      523 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/bin/cert-fingerprints.sh
--rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)    15499 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/bin/chain.py
--rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)     6132 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/bin/fling.py
--rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)    11834 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/bin/guard.py
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-03-15 18:09:31.289784 pan-chainguard-0.0.0/pan_chainguard/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      815 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/pan_chainguard/__init__.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2475 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/pan_chainguard/crtsh.py
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-03-15 18:09:31.289784 pan-chainguard-0.0.0/pan_chainguard.egg-info/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2707 2024-03-15 18:09:31.000000 pan-chainguard-0.0.0/pan_chainguard.egg-info/PKG-INFO
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      351 2024-03-15 18:09:31.000000 pan-chainguard-0.0.0/pan_chainguard.egg-info/SOURCES.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)        1 2024-03-15 18:09:31.000000 pan-chainguard-0.0.0/pan_chainguard.egg-info/dependency_links.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)       34 2024-03-15 18:09:31.000000 pan-chainguard-0.0.0/pan_chainguard.egg-info/requires.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)       15 2024-03-15 18:09:31.000000 pan-chainguard-0.0.0/pan_chainguard.egg-info/top_level.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)       90 2024-03-15 18:05:31.000000 pan-chainguard-0.0.0/pyproject.toml
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      714 2024-03-15 18:09:31.289784 pan-chainguard-0.0.0/setup.cfg
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-04-09 18:56:03.009316 pan-chainguard-0.1.0/
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      883 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/LICENSE.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2707 2024-04-09 18:56:03.009316 pan-chainguard-0.1.0/PKG-INFO
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2172 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/README.rst
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-04-09 18:56:02.999315 pan-chainguard-0.1.0/bin/
+-rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)      523 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/bin/cert-fingerprints.sh
+-rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)    17463 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/bin/chain.py
+-rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)     6315 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/bin/fling.py
+-rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)    12065 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/bin/guard.py
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-04-09 18:56:02.999315 pan-chainguard-0.1.0/pan_chainguard/
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      815 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/pan_chainguard/__init__.py
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2475 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/pan_chainguard/crtsh.py
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2024-04-09 18:56:03.009316 pan-chainguard-0.1.0/pan_chainguard.egg-info/
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2707 2024-04-09 18:56:02.000000 pan-chainguard-0.1.0/pan_chainguard.egg-info/PKG-INFO
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      351 2024-04-09 18:56:02.000000 pan-chainguard-0.1.0/pan_chainguard.egg-info/SOURCES.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)        1 2024-04-09 18:56:02.000000 pan-chainguard-0.1.0/pan_chainguard.egg-info/dependency_links.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)       34 2024-04-09 18:56:02.000000 pan-chainguard-0.1.0/pan_chainguard.egg-info/requires.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)       15 2024-04-09 18:56:02.000000 pan-chainguard-0.1.0/pan_chainguard.egg-info/top_level.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)       90 2024-04-09 18:55:07.000000 pan-chainguard-0.1.0/pyproject.toml
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      714 2024-04-09 18:56:03.009316 pan-chainguard-0.1.0/setup.cfg
```

### Comparing `pan-chainguard-0.0.0/LICENSE.txt` & `pan-chainguard-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pan-chainguard-0.0.0/PKG-INFO` & `pan-chainguard-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-chainguard
-Version: 0.0.0
+Version: 0.1.0
 Summary: Preload Trusted CA Intermediate Certificate Chains on PAN-OS
 Home-page: https://github.com/PaloAltoNetworks/pan-chainguard
 Author: Palo Alto Networks, Inc.
 Author-email: devrel@paloaltonetworks.com
 License: ISC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pan-chainguard-0.0.0/README.rst` & `pan-chainguard-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pan-chainguard-0.0.0/bin/cert-fingerprints.sh` & `pan-chainguard-0.1.0/bin/cert-fingerprints.sh`

 * *Files identical despite different names*

### Comparing `pan-chainguard-0.0.0/bin/chain.py` & `pan-chainguard-0.1.0/bin/chain.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,51 +43,57 @@
 args = None
 
 
 def main():
     global args
     args = parse_args()
 
-    asyncio.run(main_loop())
+    ret = asyncio.run(main_loop())
 
-    sys.exit(0)
+    sys.exit(ret)
 
 
 async def main_loop():
     create_archive(test=True)
 
-    invalid, roots, intermediates, parents = get_certs()
-    if args.verbose:
+    certs, invalid, roots, intermediates, parents = get_certs()
+    if args.debug:
         print('roots %d, intermediates %d, parents %d' %
               (len(roots), len(intermediates), len(parents)))
 
     chains = get_cert_chains(roots, intermediates, parents)
-    if args.verbose:
+    if args.debug > 1:
         print('chains %d (root=>intermediates)' % len(chains),
               pprint.pformat(chains),
               file=sys.stderr)
 
     total, total_invalid, panos = await get_panos_intermediates(
-        chains, invalid)
+        certs, chains, invalid)
+    print('%d invalid PAN-OS certificates found' % total_invalid)
     print('%d intermediate chains found for %d PAN-OS trusted CAs' % (
         len(panos), total))
-    if args.verbose:
+    if args.debug > 1:
         print('PAN-OS intermediate chains', pprint.pformat(panos),
               file=sys.stderr)
 
     errors, certificates = await get_cert_files(panos)
     if errors:
-        print('Warning: %d certificates were not downloaded')
+        print('Error: %d certificates were not downloaded' % errors)
+    else:
+        print('All %d certificate chains were downloaded successfully'
+              % len(certificates))
 
-    if False and args.verbose:
+    if args.debug > 2:
         print('PAN-OS certificates', pprint.pformat(certificates),
               file=sys.stderr)
 
     create_archive(certificates)
 
+    return 2 if errors else 0
+
 
 def get_certs():
     invalid = {}
     roots = []
     intermediates = []
     parents = defaultdict(list)
     certs = {}
@@ -102,40 +108,40 @@
             for row in reader:
                 sha256 = row['SHA-256 Fingerprint']
 
                 if row['Revocation Status'] not in ['', 'Not Revoked']:
                     x = '%s %s %s' % (row['Revocation Status'],
                                       sha256,
                                       row['Certificate Name'])
-                    if args.verbose:
+                    if args.debug > 1:
                         print(x, file=sys.stderr)
                     invalid[sha256] = x
                     continue
 
                 fmt = '%Y.%m.%d %z'
                 valid_from = datetime.datetime.strptime(
                     row['Valid From (GMT)'] + ' +0000', fmt)
                 valid_to = datetime.datetime.strptime(
                     row['Valid To (GMT)'] + ' +0000', fmt)
                 if now < valid_from:
                     x = 'Not yet valid (valid from %s) %s %s' % (
                         row['Valid From (GMT)'],
                         sha256,
                         row['Certificate Name'])
-                    if args.verbose:
+                    if args.debug > 1:
                         print(x, file=sys.stderr)
                     invalid[sha256] = x
                     continue
 
                 if valid_to < now:
                     x = 'Expired (valid to %s) %s %s' % (
                         row['Valid To (GMT)'],
                         sha256,
                         row['Certificate Name'])
-                    if args.verbose:
+                    if args.debug > 1:
                         print(x, file=sys.stderr)
                     invalid[sha256] = x
                     continue
 
                 derived_trust_bits = row['Derived Trust Bits']
                 if (derived_trust_bits and 'Server Authentication' not in
                    derived_trust_bits.split(';')):
@@ -156,124 +162,154 @@
                 if cert_type == 'Root Certificate':
                     roots.append(sha256)
 
                 if cert_type == 'Intermediate Certificate':
                     parent_sha256 = row['Parent SHA-256 Fingerprint']
                     if not parent_sha256:
                         x = 'Intermediate with no parent: %s' % sha256
-                        if args.verbose:
+                        if args.debug > 1:
                             print(x, file=sys.stderr)
                             invalid[sha256] = x
                         continue
 
                     intermediates.append(sha256)
                     parents[parent_sha256].append(sha256)
 
     except OSError as e:
         print('%s: %s' % (args.ccadb, e), file=sys.stderr)
         sys.exit(1)
 
-    if args.verbose:
+    if args.debug:
         for sha256 in duplicates:
             print('Duplicate certificates %s' % sha256, file=sys.stderr)
             for x in duplicates[sha256]:
                 print('  %s %s %s' % (x['Certificate Name'],
                                       x['Certificate Record Type'],
                                       x['Salesforce Record ID']),
                       file=sys.stderr)
 
-    return invalid, roots, intermediates, parents
+    return certs, invalid, roots, intermediates, parents
 
 
 def get_cert_chains(roots, intermediates, parents):
     chains = {}
 
     for k in roots:
         if k not in parents:
-            if args.verbose:
+            if args.debug:
                 print('Root with no child %s' % k,
                       file=sys.stderr)
             continue
 
         for child in parents[k]:
             chain = [k]
             follow(chain, child, parents)
-            if args.verbose:
+            if args.debug > 1:
                 print('chain[%d]:' % len(chain),
                       pprint.pformat(chain), file=sys.stderr)
 
         chains[chain[0]] = chain
 
     return chains
 
 
 def follow(chain, k, parents):
-    if args.verbose:
+    if args.debug > 1:
         print('follow[%d]:' % len(chain), k, file=sys.stderr)
 
     chain.append(k)
     if k in parents:
         for child in parents[k]:
             follow(chain, child, parents)
 
 
-async def get_panos_intermediates(chains, invalid):
+async def get_panos_intermediates(certs, chains, invalid):
     intermediates = {}
+    not_in_common_store = {}
     total = 0
     total_invalid = 0
 
     if args.fingerprints:
         try:
             with open(args.fingerprints, 'r', newline='') as csvfile:
                 reader = csv.DictReader(csvfile,
                                         dialect='unix')
                 for row in reader:
                     sha256 = row['sha256']
                     if sha256 in invalid:
                         print('Invalid PAN-OS certificate %s: %s' % (
                             row['filename'],
-                            invalid[sha256]))
+                            invalid[sha256]), file=sys.stderr)
+                        total_invalid += 1
+                        continue
+
+                    if sha256 not in certs:
+                        print('Invalid PAN-OS certificate %s: %s' % (
+                            row['filename'],
+                            'Not found in CCADB'), file=sys.stderr)
                         total_invalid += 1
                         continue
+                    else:
+                        status_root = certs[sha256]['Status of Root Cert']
+                        statuses = status_root.split(';')
+                        included = [': Included' in x for x in statuses]
+                        if not any(included):
+                            not_in_common_store[sha256] = status_root
+                            print('PAN-OS certificate not in common root store'
+                                  ' %s: %s' % (row['filename'], status_root),
+                                  file=sys.stderr)
 
                     total += 1
                     if sha256 in chains:
                         intermediates[row['filename']] = [(ROOT, sha256)]
                         for x in chains[sha256][1:]:
                             intermediates[row['filename']].append(
                                 (INTERMEDIATE, x))
+                    elif args.verbose:
+                        x = '%s %s' % (row['filename'], 'intermediates 0')
+                        if sha256 in not_in_common_store:
+                            x += ' (not in common root store)'
+                        print(x, file=sys.stderr)
 
         except OSError as e:
-            print('%s: %s' % (args.ccadb, e), file=sys.stderr)
+            print('%s: %s' % (args.fingerprints, e), file=sys.stderr)
             sys.exit(1)
 
     return total, total_invalid, intermediates
 
 
 async def download(api, sequence, sha256):
     tries = 0
     MAX_TRIES = 5
     RETRY_SLEEP = 5.0
 
+    RETRY_STATUS = [
+        429,  # Too Many Requests
+        502,  # Bad Gateway
+        504,  # Gateway Time-out
+    ]
+
     while True:
         tries += 1
         try:
             resp = await api.download(id=sha256[1])
 
-            if resp.status == 429:
-                x = '%d %s' % (resp.status, resp.reason)
+            if resp.status in RETRY_STATUS:
+                x = '%d %s %s %s' % (
+                    resp.status, resp.reason, sequence, sha256[1])
                 if tries == MAX_TRIES:
-                    print('no retry after try %d, %s' % (tries, x),
+                    print('no retry after try %d %s' % (tries, x),
                           file=sys.stderr)
+                    x = 'download failed ' + x
                     break
-                print('retry after try %d, %s' % (tries, x),
+                print('retry after try %d %s' % (tries, x),
                       file=sys.stderr)
                 await asyncio.sleep(RETRY_SLEEP)
             elif resp.status != 200:
-                x = 'download %d %s %s %s' % (
+                x = 'download failed %d %s %s %s' % (
                     resp.status, resp.reason, sequence, sha256[1])
                 break
             else:
                 filename, content = await api.content(resp=resp)
                 if filename is None:
                     filename = sha256[1] + '.crt'
 
@@ -283,31 +319,33 @@
                    content.endswith(end)):
                     return filename, content, sequence, sha256[0]
                 else:
                     # XXX ephemeral?
                     x = 'content malformed %s %s %s' % (
                         sequence, sha256[1], content)
                     if tries == MAX_TRIES:
-                        print('no retry after try %d, %s' % (tries, x),
+                        print('no retry after try %d %s' % (tries, x),
                               file=sys.stderr)
+                        x = 'download failed ' + x
                         break
-                    print('retry after try %d, %s' % (tries, x),
+                    print('retry after try %d %s' % (tries, x),
                           file=sys.stderr)
                     await asyncio.sleep(RETRY_SLEEP)
 
         except (asyncio.TimeoutError,
                 asyncio.CancelledError,  # XXX
                 aiohttp.ClientError) as e:
             msg = e if str(e) else type(e).__name__
-            x = 'CrtShApi: %s: %s %s' % (msg, sequence, sha256[1])
+            x = 'CrtShApi: %s %s %s' % (msg, sequence, sha256[1])
             if tries == MAX_TRIES:
-                print('no retry after try %d, %s' % (tries, x),
+                print('no retry after try %d %s' % (tries, x),
                       file=sys.stderr)
+                x = 'download failed ' + x
                 break
-            print('retry after try %d, %s' % (tries, x),
+            print('retry after try %d %s' % (tries, x),
                   file=sys.stderr)
             # no sleep
 
         except ArgsError as e:
             x = 'CrtShApi: %s' % e
             break
 
@@ -335,32 +373,33 @@
     total = 0
     errors = 0
 
     for sequence in roots:
         sequence_friendly = sequence
         if sequence.endswith('.cer'):
             sequence_friendly = sequence[:-4]
-        print('download CA %s intermediates %d' % (sequence_friendly,
-                                                   len(roots[sequence][1:])),
-              flush=True)
+        if args.verbose:
+            print('download %s intermediates %d' % (
+                sequence_friendly,
+                len(roots[sequence][1:])))
 
         for sha256 in roots[sequence]:
             if not args.roots and sha256[0] == ROOT:
                 continue
             total += 1
             tasks.append(download(api, sequence_friendly, sha256))
 
             if len(tasks) == MAX_TASKS:
                 errors += await run_tasks(tasks, certificates)
                 tasks = []
 
     if len(tasks):
         errors += await run_tasks(tasks, certificates)
 
-    if args.verbose:
+    if args.debug:
         end = time.time()
         elapsed = end - start
         mins = elapsed // 60
         secs = elapsed % 60
         avg = elapsed / total if total > 0 else 0
         print('%d tasks, elapsed %.2f seconds, %dm%ds, avg %.2fs' %
               (total, elapsed, mins, secs, avg),
@@ -369,29 +408,29 @@
     return errors, certificates
 
 
 async def run_tasks(tasks, certificates):
     INTERVAL_WAIT = 3.3  # random throttle sweet spot to avoid TimeoutError
     errors = 0
 
-    if args.verbose:
+    if args.debug:
         print('running %d tasks' % len(tasks),
               file=sys.stderr)
         start = time.time()
 
     for coro in asyncio.as_completed(tasks):
         filename, content, sequence, cert_type = await coro
         if filename is None:
             # error
-            print(content)
+            print(content, file=sys.stderr)
             errors += 1
         else:
             certificates[sequence].append((cert_type, filename, content))
 
-    if args.verbose:
+    if args.debug:
         end = time.time()
         elapsed = end - start
         rate = len(tasks) / elapsed
         rate2 = elapsed / len(tasks)
         print('%d tasks complete, elapsed %.2f seconds, '
               '%.2f tasks/sec, %.2f secs/task' %
               (len(tasks), elapsed, rate, rate2), file=sys.stderr)
@@ -445,22 +484,27 @@
                         ' (default: %s)' % x)
     parser.add_argument('--roots',
                         action='store_true',
                         help='also download root CAs (experimental)')
     parser.add_argument('--verbose',
                         action='store_true',
                         help='enable verbosity')
+    parser.add_argument('--debug',
+                        type=int,
+                        choices=[0, 1, 2, 3],
+                        default=0,
+                        help='enable debug')
     x = '%s %s' % (title, __version__)
     parser.add_argument('--version',
                         action='version',
                         help='display version',
                         version=x)
     args = parser.parse_args()
 
-    if args.verbose:
+    if args.debug:
         print(args, file=sys.stderr)
 
     return args
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pan-chainguard-0.0.0/bin/fling.py` & `pan-chainguard-0.1.0/bin/fling.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 
     create_archive(test=True)
 
     store = {}
     for cert_name, filename in get_trusted_certs(xapi):
         if args.verbose:
             print('Exporting %s => %s' % (cert_name, filename))
-        filename2, content = export_cert(xapi, cert_name)
-        if filename2 is not None:
+        _, content = export_cert(xapi, cert_name)
+        if content is not None:
             store[filename] = content
 
     total = create_archive(store)
     print('Exported %d PAN-OS trusted CAs to %s' % (total, args.certs))
 
 
 def get_trusted_certs(xapi):
@@ -185,22 +185,27 @@
                         type=int,
                         choices=[0, 1, 2, 3],
                         default=0,
                         help='pan.xapi debug')
     parser.add_argument('--verbose',
                         action='store_true',
                         help='enable verbosity')
+    parser.add_argument('--debug',
+                        type=int,
+                        choices=[0, 1, 2, 3],
+                        default=0,
+                        help='enable debug')
     x = '%s %s' % (title, __version__)
     parser.add_argument('--version',
                         action='version',
                         help='display version',
                         version=x)
     args = parser.parse_args()
 
-    if args.verbose:
+    if args.debug:
         print(args, file=sys.stderr)
 
     return args
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pan-chainguard-0.0.0/bin/guard.py` & `pan-chainguard-0.1.0/bin/guard.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,34 +276,35 @@
     elif panorama:
         partial.append(shared_object)
     else:
         partial.append(device_and_network)
         partial.append(policy_and_objects)
 
     cmd = etree.tostring(root).decode()
-    if args.verbose:
+    if args.debug:
         print(cmd, file=sys.stderr)
 
     kwargs = {
         'cmd': cmd,
         'sync': True,
     }
 
-    print('commit config for admin %s' % args.admin)
-    api_request(xapi, xapi.commit, kwargs, 'success')
     if args.verbose:
+        print('commit config for admin %s' % args.admin)
+    api_request(xapi, xapi.commit, kwargs, 'success')
+    if args.debug:
         print(xapi.xml_root(), file=sys.stderr)
 
     if xapi.status_code is not None:
         code = ' [code=\"%s\"]' % xapi.status_code
     else:
         code = ''
     if xapi.status is not None:
         print('commit: %s%s' % (xapi.status, code), end='')
-    if xapi.status_detail is not None:
+    if args.verbose and xapi.status_detail is not None:
         print(': "%s"' % xapi.status_detail.rstrip(), end='')
     print()
 
 
 def s1_in_s2(s1, s2):
     if isinstance(s2, str):
         return s1 == s2
@@ -352,22 +353,27 @@
                         type=int,
                         choices=[0, 1, 2, 3],
                         default=0,
                         help='pan.xapi debug')
     parser.add_argument('--verbose',
                         action='store_true',
                         help='enable verbosity')
+    parser.add_argument('--debug',
+                        type=int,
+                        choices=[0, 1, 2, 3],
+                        default=0,
+                        help='enable debug')
     x = '%s %s' % (title, __version__)
     parser.add_argument('--version',
                         action='version',
                         help='display version',
                         version=x)
     args = parser.parse_args()
 
-    if args.verbose:
+    if args.debug:
         print(args, file=sys.stderr)
 
     return args
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pan-chainguard-0.0.0/pan_chainguard/__init__.py` & `pan-chainguard-0.1.0/pan_chainguard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 
-__version__ = '0.0.0'
+__version__ = '0.1.0'
 title = 'pan-chainguard'
```

### Comparing `pan-chainguard-0.0.0/pan_chainguard/crtsh.py` & `pan-chainguard-0.1.0/pan_chainguard/crtsh.py`

 * *Files identical despite different names*

### Comparing `pan-chainguard-0.0.0/pan_chainguard.egg-info/PKG-INFO` & `pan-chainguard-0.1.0/pan_chainguard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-chainguard
-Version: 0.0.0
+Version: 0.1.0
 Summary: Preload Trusted CA Intermediate Certificate Chains on PAN-OS
 Home-page: https://github.com/PaloAltoNetworks/pan-chainguard
 Author: Palo Alto Networks, Inc.
 Author-email: devrel@paloaltonetworks.com
 License: ISC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pan-chainguard-0.0.0/setup.cfg` & `pan-chainguard-0.1.0/setup.cfg`

 * *Files identical despite different names*

