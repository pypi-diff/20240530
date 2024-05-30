# Comparing `tmp/muttfuzz-0.8.8-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10244 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    11144 b- defN 24-May-28 18:05 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     6186 b- defN 24-May-29 13:56 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6941 b- defN 24-May-29 13:56 muttfuzz-0.8.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 13:56 muttfuzz-0.8.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-29 13:56 muttfuzz-0.8.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-29 13:56 muttfuzz-0.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-29 13:56 muttfuzz-0.8.8.dist-info/RECORD
-8 files, 30000 bytes uncompressed, 9160 bytes compressed:  69.5%
+Zip file size: 10607 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     5184 b- defN 24-May-30 15:09 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx    11881 b- defN 24-May-30 15:09 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     6630 b- defN 24-May-30 15:09 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     6941 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-30 15:09 muttfuzz-0.8.9.dist-info/RECORD
+8 files, 31421 bytes uncompressed, 9523 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.8.dist-info/METADATA
+Filename: muttfuzz-0.8.9.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.8.dist-info/WHEEL
+Filename: muttfuzz-0.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.8.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.8.dist-info/top_level.txt
+Filename: muttfuzz-0.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.8.dist-info/RECORD
+Filename: muttfuzz-0.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -41,14 +41,16 @@
                         help='timeout for post-mutant command')
     parser.add_argument('--status_cmd', type=str, default="",
                         help='command to execute to show fuzzing stats')
     parser.add_argument('--order', type=int, default=1,
                         help='mutation order (default 1)')
     parser.add_argument('-s', '--score', action='store_true',
                         help="compute a mutation score, instead of fuzzing.")
+    parser.add_argument('--save_mutants', type=str, default="",
+                        help='directory in which to save generated mutants/checks; no saving if not provided or empty')
 
     parsed_args = parser.parse_args(sys.argv[1:])
     return (parsed_args, parser)
 
 
 def make_config(pargs):
     """
@@ -81,15 +83,16 @@
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.post_mutant_timeout,
                                    config.status_cmd,
                                    config.order,
-                                   config.score)
+                                   config.score,
+                                   config.save_mutants)
     except IndexError:
         print("Target binary seems to have no jumps, so mutation will not do anything!")
 
 
 
 if __name__ == "__main__":
     main()
```

## muttfuzz/fuzzutil.py

```diff
@@ -33,14 +33,16 @@
         f.write(executable_code)
     os.rename("/tmp/restore_executable", executable)
     subprocess.check_call(['chmod', '+x', executable])
 
 
 def silent_run_with_timeout(cmd, timeout):
     dnull = open(os.devnull, 'w')
+    print("*" * 80)
+    print("EXECUTING", cmd)
     start_P = time.time()
     try:
         with open("cmd_errors.txt", 'w') as cmd_errors:
             P = subprocess.Popen(cmd, shell=True, preexec_fn=os.setsid,
                                  stdout=dnull, stderr=cmd_errors)
             while (P.poll() is None) and ((time.time() - start_P) < timeout):
                 time.sleep(min(0.5, timeout / 10.0)) # Allow for small timeouts
@@ -52,15 +54,19 @@
             except:
                 cmd_errors_out = "ERROR READING OUTPUT"
         if len(cmd_errors_out) > 0:
             print("OUTPUT (TRUNCATED TO LAST 20 LINES):")
             print("\n".join(cmd_errors_out.split("\n")[-20:]))
     finally:
         if P.poll() is None:
+            print("KILLING SUBPROCESS DUE TO TIMEOUT")
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
+    print("COMPLETE IN", round(time.time() - start_P, 2), "SECONDS")
+    print("*" * 80)
+
     return P.returncode
 
 
 def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
                       only_mutate=[],
                       avoid_mutating=[],
                       reachability_check_cmd="",
@@ -70,17 +76,29 @@
                       initial_fuzz_cmd="",
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
                       post_mutant_timeout=2.0,
                       status_cmd="",
                       order=1,
-                      score=False):
+                      score=False,
+                      save_mutants=""):
     executable_code = mutate.get_code(executable)
     executable_jumps = mutate.get_jumps(executable, only_mutate, avoid_mutating)
+    print("FOUND", len(executable_jumps), "JUMPS")
+    print("JUMPS BY SECTION:")
+    section_jumps = {}
+    for jump in executable_jumps:
+        if jump["section_name"] not in section_jumps:
+            section_jumps[jump["section_name"]] = [jump]
+        else:
+            section_jumps[jump["section_name"]].append(jump)
+    for section in section_jumps:
+        print(section, len(section_jumps[section]))
+    print()
     start_fuzz = time.time()
     mutant_no = 1
     try:
         if initial_fuzz_cmd != "":
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
@@ -107,15 +125,16 @@
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
             print(round(time.time() - start_fuzz, 2),
                   "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
             mutant_no += 1
             # make a new mutant of the executable; rename avoids hitting a busy executable
             mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order,
-                               reachability_filename=reachability_filename)
+                               reachability_filename=reachability_filename, save_mutants=save_mutants,
+                               save_count = mutant_no)
             mutant_ok = True
             if reachability_check_cmd != "":
                 print("CHECKING REACHABILITY")
                 reachability_checks += 1.0
                 os.rename(reachability_filename, executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout)
```

## muttfuzz/mutate.py

```diff
@@ -128,22 +128,27 @@
                 reach_code[loc + offset] = NOP[0]
             new_code[loc + offset] = new_data[offset]
     return (new_code, reach_code)
 
 def mutant(filename, order=1, avoid_mutating=[]):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
-def mutate_from(code, jumps, new_filename, order=1, reachability_filename=""):
-    (m, r) = mutant_from(code, jumps, order=order)
-    with open(new_filename, 'wb') as f:
-        f.write(m)
+def write_files(mutant, reach, new_filename, reachability_filename="", save_mutants="", save_count=0):
+    with open(new_filename, "wb") as f:
+        f.write(mutant)
+    if save_mutants != "":
+        with open(save_mutants + "/mutant_" + str(save_count), "wb") as f:
+            f.write(mutant)
     if reachability_filename != "":
         with open(reachability_filename, "wb") as f:
-            f.write(r)
+            f.write(reach)
+        if save_mutants != "":
+            with open(save_mutants + "/reach_" + str(save_count), "wb") as f:
+                f.write(reach)
+
+def mutate_from(code, jumps, new_filename, order=1, reachability_filename="", save_mutants="", save_count=0):
+    (m, r) = mutant_from(code, jumps, order=order)
+    write_files(m, r, new_filename, reachability_filename, save_mutants, save_count)
 
-def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_filename=""):
+def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_filename="", save_mutants="", save_count=0):
     (m, r) = mutant(filename, order=order, avoid_mutating=avoid_mutating)
-    with open(new_filename, "wb") as f:
-        f.write(m)
-    if reachability_filename != "":
-        with open(reachability_filename, "wb") as f:
-            f.write(r)
+    write_files(m, r, new_filename, reachability_filename, save_mutants, save_count)
```

## Comparing `muttfuzz-0.8.8.dist-info/METADATA` & `muttfuzz-0.8.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.8
+Version: 0.8.9
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

