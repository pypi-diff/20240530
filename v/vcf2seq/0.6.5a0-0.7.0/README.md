# Comparing `tmp/vcf2seq-0.6.5a0.tar.gz` & `tmp/vcf2seq-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcf2seq-0.6.5a0.tar", last modified: Tue May  7 14:14:49 2024, max compression
+gzip compressed data, was "vcf2seq-0.7.0.tar", last modified: Thu May 30 09:47:58 2024, max compression
```

## Comparing `vcf2seq-0.6.5a0.tar` & `vcf2seq-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.6.5a0/LICENCE.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.6.5a0/MANIFEST.in
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.6.5a0/README.md
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/setup.cfg
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.6.5a0/setup.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/vcf2seq/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      165 2024-05-06 08:56:10.000000 vcf2seq-0.6.5a0/vcf2seq/__init__.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.6.5a0/vcf2seq/ascii.py
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      246 2024-05-07 14:13:54.000000 vcf2seq-0.6.5a0/vcf2seq/info.py
--rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    14023 2024-05-07 14:12:48.000000 vcf2seq-0.6.5a0/vcf2seq/vcf2seq.py
-drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-07 14:14:49.499539 vcf2seq-0.6.5a0/vcf2seq.egg-info/
--rw-r--r--   0 benoit    (1001) bio2m     (1010)     2331 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/PKG-INFO
--rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/SOURCES.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/dependency_links.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/entry_points.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/requires.txt
--rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-07 14:14:49.000000 vcf2seq-0.6.5a0/vcf2seq.egg-info/top_level.txt
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-30 09:47:58.978331 vcf2seq-0.7.0/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)    34916 2023-03-07 08:59:59.000000 vcf2seq-0.7.0/LICENCE.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       98 2024-04-09 10:58:25.000000 vcf2seq-0.7.0/MANIFEST.in
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2329 2024-05-30 09:47:58.978331 vcf2seq-0.7.0/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     1708 2024-05-06 09:01:58.000000 vcf2seq-0.7.0/README.md
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       38 2024-05-30 09:47:58.978331 vcf2seq-0.7.0/setup.cfg
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      990 2024-04-10 14:28:47.000000 vcf2seq-0.7.0/setup.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-30 09:47:58.978331 vcf2seq-0.7.0/vcf2seq/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      152 2024-05-30 09:47:49.000000 vcf2seq-0.7.0/vcf2seq/__init__.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)     2393 2023-07-13 15:02:22.000000 vcf2seq-0.7.0/vcf2seq/ascii.py
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      240 2024-05-30 09:44:35.000000 vcf2seq-0.7.0/vcf2seq/info.py
+-rwxr-xr-x   0 benoit    (1001) bio2m     (1010)    14276 2024-05-29 16:48:12.000000 vcf2seq-0.7.0/vcf2seq/vcf2seq.py
+drwxr-xr-x   0 benoit    (1001) bio2m     (1010)        0 2024-05-30 09:47:58.978331 vcf2seq-0.7.0/vcf2seq.egg-info/
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)     2329 2024-05-30 09:47:58.000000 vcf2seq-0.7.0/vcf2seq.egg-info/PKG-INFO
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)      301 2024-05-30 09:47:58.000000 vcf2seq-0.7.0/vcf2seq.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        1 2024-05-30 09:47:58.000000 vcf2seq-0.7.0/vcf2seq.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)       49 2024-05-30 09:47:58.000000 vcf2seq-0.7.0/vcf2seq.egg-info/entry_points.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-30 09:47:58.000000 vcf2seq-0.7.0/vcf2seq.egg-info/requires.txt
+-rw-r--r--   0 benoit    (1001) bio2m     (1010)        8 2024-05-30 09:47:58.000000 vcf2seq-0.7.0/vcf2seq.egg-info/top_level.txt
```

### Comparing `vcf2seq-0.6.5a0/LICENCE.md` & `vcf2seq-0.7.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.5a0/PKG-INFO` & `vcf2seq-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.5a0
+Version: 0.7.0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `vcf2seq-0.6.5a0/README.md` & `vcf2seq-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.5a0/setup.py` & `vcf2seq-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.5a0/vcf2seq/ascii.py` & `vcf2seq-0.7.0/vcf2seq/ascii.py`

 * *Files identical despite different names*

### Comparing `vcf2seq-0.6.5a0/vcf2seq/vcf2seq.py` & `vcf2seq-0.7.0/vcf2seq/vcf2seq.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,92 +29,104 @@
         chr_dict = pyfaidx.Fasta(args.genome) # if fai file doesn't exists, it will be automatically created
     except pyfaidx.FastaNotFoundError as err:
         sys.exit(f"FastaNotFoundError: {err}")
     except OSError as err:
         sys.exit(f"\n{COL.RED}WriteError: directory {os.path.dirname(args.genome)!r} may not be "
                   "writable.\nIf you can't change the rights, you can create a symlink and target "
                   f"it. For example:\n  ln -s {args.genome} $HOME\n{COL.END}")
-    vcf_ok, vcf_msg = input_ctrl(args, chr_dict)
-    if not vcf_ok:
-        sys.exit(f"{COL.RED}{vcf_msg}")
-    results, warnings = compute(args, chr_dict)
-    write(args, results, warnings)
+    # ~ vcf_ok, vcf_msg = input_ctrl(args, chr_dict)
+    # ~ if not vcf_ok:
+        # ~ sys.exit(f"{COL.RED}{vcf_msg}")
+    resp = compute(args, chr_dict)
+    output(args, resp)
 
 
-def input_ctrl(args, chr_dict):
-    with open(args.input.name) as fh:
-        for row in fh:
-            if row.startswith('#'):
-                continue
-            try:
-                chr, pos, id, ref, alt, *rest = row.rstrip('\n').split('\t')
-            except ValueError:
-                msg = ("ErrorVcfFormat: not enough columns for a vcf (expected at least 5).")
-                return False, msg
-
-            ### Check some commonly issues
-            if not pos.isdigit():
-                msg = (f"ErrorVcfFormat: second column is the position. It must be a "
-                         f"digit (found: {pos!r}).\n"
-                          "A commonly issue is that the header is not commented by a '#' ")
-                return False, msg
-            if chr not in chr_dict:
-                msg (f"{COL.RED}ErrorChr: Chromosomes are not named in the same way in the "
-                          "query and the genome file. Below the first chromosome found: \n"
-                         f" your query: {chr}\n"
-                         f" genome: {next(iter(chr_dict.keys()))}\n"
-                         f"Please, correct your request (or modify the file '{args.genome}.fai').")
-                return False, msg
-            break
+def _input_ok(args, rows, resp, chr_dict):
+    for row in rows:
+        if row.startswith('#'):
+            continue
+        try:
+            chr, pos, id, ref, alt, *rest = row.rstrip('\n').split('\t')
+        except ValueError:
+            resp["error"] = ("ErrorVcfFormat: not enough columns for a vcf (expected at least 5).")
+            resp["is_ok"] = False
+            return False
+
+        ### Check some commonly issues
+        if not pos.isdigit():
+            resp["error"] = (f"ErrorVcfFormat: second column is the position. It must be a "
+                     f"digit (found: {pos!r}).\n"
+                      "A commonly issue is that the header is not commented by a '#' ")
+            rest["is_ok"] = False
+            return False
+        if chr not in chr_dict:
+            resp["error"] = ("ErrorChr: Chromosomes are not named in the same way in the "
+                      "query and the genome file. Below the first chromosome found: \n"
+                     f" your query: {chr}\n"
+                     f" genome: {next(iter(chr_dict.keys()))}\n"
+                     f"Please, correct your request (or modify the file '{args.genome}.fai').")
+            rest["is_ok"] = False
+            return False
+        break
     return True, "ok"
 
 
 def compute(args, chr_dict):
+    ### object to return
+    resp = {
+        "is_ok": True,
+        "result": [],
+        "warning": [],
+        "error": None
+        }
+
+    ### convert file as list
+    rows = args.input.read().splitlines()
+    
+    ### check file syntax
+    if not _input_ok(args, rows, resp, chr_dict):
+        return resp
+        
+
     res_ref = []
     res_alt = []
-    warnings = []
-    num_row = 0
+    valid_nuc = ["A", "T", "C", "G", args.blank]
     cols_id = ascii.get_index(args.add_columns)    # columns chars are converted as index, ex: AA -> 27
-    for variant in args.input:
-        num_row += 1
-        if not variant.rstrip('\n') or variant.startswith('#'):
+    
+    for i,row in enumerate(rows):
+        if not row or row.startswith('#'):
             continue
-        fields = variant.rstrip('\n').split('\t')
+        fields = row.split('\t')
         chr, position, id, ref, alts = fields[:5]
 
         ### check if --add-columns is compatible with number of columns
         if args.add_columns and max(cols_id) > len(fields):
-            warnings.append(f"Error: vcf file has {len(fields)} columns, but you asked for "
-                  f"{max(args.add_columns)} (line {num_row}).")
-            return None, warnings
+            resp["error"] = (f"Error: vcf file has {len(fields)} columns, but you asked for "
+                  f"{max(args.add_columns)}.")
+            resp["is_ok"] = False
+            return resp
 
         alts = alts.split(',')
         for alt in alts:
 
-            ''' using genome broseable syntax (but miss original information)
-            mid_l = mid_r = args.size // 2
-            if not args.size&1: mid_l -= 1
-            header = f"chr{chr}:{int(position)-mid_l}-{int(position)+mid_r}_{ref}_{alt}"
-            '''
             header = f"{chr}:{position}_{ref}_{alt}"
             tsv_cols =  '\t' + '\t'.join([chr, position, ref, alt]) if args.output_format == 'tsv' else ''
 
-
             ### WARNING: event bigger than kmer size
-            if max(len(ref), len(alt)) > args.size :
-                warnings.append(f"Warning: large alteration ({chr}_{position}_{ref}_{alt}), truncated in output.")
+            if len(ref) > args.size :
+                resp["warning"].append(f" REF deletion larger than {args.size} at line {i+1}, truncated in output ({ref}).")
 
-
-            ### ERROR: REF base is not valid
-            NUC = ["A", "T", "C", "G", args.blank]
-            for nuc in (ref[0], alt[0]):
-                if nuc not in NUC:
-                    warnings.append(f"Warning: REF base {nuc!r} is not valid at line {num_row}, ignored.\n"
-                            f"        You might add the '--blank {nuc}' option or check your VCF file."
-                            )
+            ### ERROR: REF/ALT base is not valid
+            bad_nuc = [ a for a in (alt[0], ref[0]) if a not in valid_nuc]
+            if bad_nuc:
+                bad_nuc = bad_nuc[0]
+                resp["warning"].append(f" The base {bad_nuc!r} is not valid at line {i+1}, ignored.\n"
+                        f"    You might add the '--blank {bad_nuc}' option or check your VCF file."
+                        )
+                continue
 
             #####################################################################################
             #                Some explanations on variable naming                               #
             #                                                                                   #
             #  l = length                                                                       #
             #  ps = position start                                                              #
             #  pe = position end                                                                #
@@ -160,25 +172,25 @@
                 ps_alt3 = ps_ref2 + l_ref2
                 pe_alt3 = ps_alt3 + l_alt3
                 seq_alt1 = chr_dict[chr][ps_alt1:ps_ref2]
                 alt = alt if alt != args.blank else ""
                 seq_alt3 = chr_dict[chr][ps_alt3:pe_alt3]
                 alt_seq = f"{seq_alt1}{alt}{seq_alt3}"
             except:
-                warnings.append(f"Warning: something went wrong at line {num_row}, ignored.")
+                resp["warning"].append(f"Warning: something went wrong at line {num_row}, ignored.")
                 break
 
             ### WARNING: REF bases must be the same as the calculated position
             seq_ref2 = chr_dict[chr][ps_ref2:ps_ref2+l_ref2]
             if l_ref2 and not ref == seq_ref2:
-                warnings.append("Warning: mismatch between REF and genome "
-                                f"at line {num_row} (chr{chr}:{ps_ref2+1}).\n"
-                                f"    - REF in the vcf file: {ref!r}\n"
-                                f"    - Found in the genome: '{seq_ref2}'\n"
-                                "    Please check if the given genome is appropriate.")
+                resp["warning"].append(" Mismatch between REF and genome "
+                                f"at line {i+1} (chr{chr}:{ps_ref2+1}).\n"
+                                f"   - REF in the vcf file: {ref!r}\n"
+                                f"   - Found in the genome: '{seq_ref2}'\n"
+                                "   Please check if the given genome is appropriate.")
             col_sep = ' ' if args.output_format == 'fa' else '\t'
 
             ### Append results in lists
             if len(ref_seq) == args.size == len(alt_seq):
                 ### append additional selected columns to the header
                 added_cols = f"{col_sep}{col_sep.join([fields[num-1] for num in cols_id])}" if cols_id else ''
                 ### append to list according of output format
@@ -187,62 +199,66 @@
                     res_alt.append(f"{alt_seq}{col_sep}{header}_alt{tsv_cols}{col_sep}alt{added_cols}")
                 else:
                     res_ref.append(f">{header}_ref{added_cols}")
                     res_ref.append(ref_seq)
                     res_alt.append(f">{header}_alt{added_cols}")
                     res_alt.append(alt_seq)
             elif len(alt_seq) > args.size:
-                warnings.append(f"Warning: ALT length ({len(alt_seq)} bp) larger than sequence "
-                                f"({args.size} bp) at line {num_row}, ignored.")
+                resp["warning"].append(f" ALT length ({len(alt_seq)} bp) larger than sequence "
+                                f"({args.size} bp) at line {i+1}, ignored.")
             else:
-                warnings.append(f"Warning: sequence size not correct at line {num_row}, ignored"
-                                "f({len(alt_seq)} != {args.size}).")
-
-    res = list()
+                resp["warning"].append(f" Sequence size not correct at line {i+1}, ignored"
+                                f"({len(alt_seq)} != {args.size}).")
+        
+            
+    # ~ res = list()
     if args.output_format == 'tsv':
         str_cols = '\t' + "col_{}".format('\tcol_'.join(args.add_columns)) if args.add_columns else ''
-        res.append(f"sequence\tid\tchr\tposition\tREF\tALT\ttype{str_cols}")
+        resp["result"].append(f"sequence\tid\tchr\tposition\tREF\tALT\ttype{str_cols}")
 
     if args.type == 'alt':
-        res += res_alt
+        resp["result"] += res_alt
     elif args.type == 'ref':
-        res += res_ref
+        resp["result"] += res_ref
     else:
         if args.output_format == 'fa':
             for i in range(0, len(res_alt), 2):
-                res += [res_ref[i], res_ref[i+1]]
-                res += [res_alt[i], res_alt[i+1]]
+                resp["result"] += [res_ref[i], res_ref[i+1]]
+                resp["result"] += [res_alt[i], res_alt[i+1]]
         else:
             for i,_ in enumerate(res_alt):
-                res.append(res_ref[i])
-                res.append(res_alt[i])
-    return res, warnings
+                resp["result"].append(res_ref[i])
+                resp["result"].append(res_alt[i])
+    return resp
 
 
 
-def write(args, results, warnings):
+def output(args, resp):
     ### OUTPUT RESULTS
     ext = args.output_format
     ## define output file
     if not args.output:
         name, _ = os.path.splitext(os.path.basename(args.input.name))
         args.output = f"{name}-vcf2seq.{ext}"
 
-    ## write results in file
-    if results:
-        with open(args.output, 'w') as fh:
-            for result in results:
-                fh.write(f"{result}\n")
-
-    ### WARNINGS
-    if warnings:
-        for warning in warnings:
-            color = COL.RED if warning.startswith('Error') else COL.PURPLE
-            print(f"{color}{warning}\n")
-        print(COL.END)
+    if resp["is_ok"]:
+        ## write results in file
+        if resp["result"]:
+            with open(args.output, 'w') as fh:
+                for result in resp["result"]:
+                    fh.write(f"{result}\n")
+        ### WARNINGS
+        if resp["warning"]:
+            print(f"{COL.PURPLE}Warnings:\n")
+            for warning in resp["warning"]:
+                for warning in resp["warning"]:
+                    print(f"{warning}\n")
+            print(COL.END)
+    else:
+        print(f"{COL.RED}{resp['error']}")
 
 
 class COL:
     PURPLE = '\033[95m'
     CYAN = '\033[96m'
     DARKCYAN = '\033[36m'
     BLUE = '\033[94m'
```

### Comparing `vcf2seq-0.6.5a0/vcf2seq.egg-info/PKG-INFO` & `vcf2seq-0.7.0/vcf2seq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcf2seq
-Version: 0.6.5a0
+Version: 0.7.0
 Summary: Inputing a VCF file, it returns the genomic sequence at the specified length (31 by default).
 Home-page: https://github.com/bio2m/vcf2seq
 Author: Benoit Guibert
 Author-email: benoit.guibert@free.fr
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

