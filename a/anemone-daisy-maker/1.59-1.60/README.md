# Comparing `tmp/anemone_daisy_maker-1.59.tar.gz` & `tmp/anemone_daisy_maker-1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemone_daisy_maker-1.59.tar", last modified: Tue May 28 05:17:44 2024, max compression
+gzip compressed data, was "anemone_daisy_maker-1.60.tar", last modified: Thu May 30 05:58:28 2024, max compression
```

## Comparing `anemone_daisy_maker-1.59.tar` & `anemone_daisy_maker-1.60.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-28 05:17:37.000000 anemone_daisy_maker-1.59/LICENSE
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7050 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/anemone/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    77301 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone/__main__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7050 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       23 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-28 05:17:44.611809 anemone_daisy_maker-1.59/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7217 2024-05-28 05:17:44.000000 anemone_daisy_maker-1.59/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-30 05:58:28.180976 anemone_daisy_maker-1.60/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-30 05:58:20.000000 anemone_daisy_maker-1.60/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7222 2024-05-30 05:58:28.180976 anemone_daisy_maker-1.60/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-30 05:58:28.180976 anemone_daisy_maker-1.60/anemone/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    78876 2024-05-30 05:58:27.000000 anemone_daisy_maker-1.60/anemone/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       33 2024-05-30 05:58:27.000000 anemone_daisy_maker-1.60/anemone/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-30 05:58:28.180976 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7222 2024-05-30 05:58:28.000000 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      316 2024-05-30 05:58:28.000000 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-30 05:58:28.000000 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-30 05:58:28.000000 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       23 2024-05-30 05:58:28.000000 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-30 05:58:28.000000 anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-30 05:58:28.180976 anemone_daisy_maker-1.60/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7389 2024-05-30 05:58:27.000000 anemone_daisy_maker-1.60/setup.py
```

### Comparing `anemone_daisy_maker-1.59/LICENSE` & `anemone_daisy_maker-1.60/LICENSE`

 * *Files identical despite different names*

### Comparing `anemone_daisy_maker-1.59/PKG-INFO` & `anemone_daisy_maker-1.60/anemone_daisy_maker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: anemone_daisy_maker
-Version: 1.59
+Name: anemone-daisy-maker
+Version: 1.60
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -14,22 +14,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
-`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce three different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It can produce four different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
 3. Text with no audio: this requires just XHTML files, and extracts all text with a specified attribute (`data-pid` by default)
 
+4. Text with some audio: this is a combination of the above two methods, and you'll need to specify `skip` in the JSON file list for the chapters that do not yet have recorded audio
+
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
 ### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
```

### Comparing `anemone_daisy_maker-1.59/anemone/__init__.py` & `anemone_daisy_maker-1.60/anemone/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Anemone 1.59 (http://ssb22.user.srcf.net/anemone)
+Anemone 1.6 (http://ssb22.user.srcf.net/anemone)
 (c) 2023-24 Silas S. Brown.  License: Apache 2
 
 To use this module, either run it from the command
 line, or import it and use the anemone() function.
 """
 
 # Licensed under the Apache License, Version 2.0 (the "License");
@@ -34,15 +34,15 @@
     of the name of a JSON file, and/or an HTML
     string instead of the name of an HTML file
     (this can also be done on the command line
     with careful quoting).
     If you do not give this function any arguments
     it will look at the system command line.
     Return value is a list of warnings, if any."""
-    
+
     R=Run(*files,**options)
     R.check()
     if R.mp3_recode or any(f.strip().lower().
                            endswith(
                                f"{os.extsep}wav")
                            for f in files
                            if isinstance(f,str)):
@@ -244,25 +244,23 @@
     R = self
     R.audioData,R.filenameTitles = [],[]
     R.jsonData = []
     R.textData,R.htmlData = [],[]
     R.imageFiles,R.outputFile = [],None
     R.warnings = []
     if inFiles: # being called as a module
-        inFiles2 = [f for f in inFiles if isinstance(f,str)]
         R.__dict__.update(
             get_argument_parser().parse_args(
-                (inFiles2 if inFiles2 else ["placeholder"]) +
+                ["placeholder"] +
                 [a for k,v in kwargs.items()
                  for a in
                  ['--'+k.replace('_','-'),str(v)]
                  if type(v) in [str,int]])
             .__dict__)
-        if not inFiles2: del R.files[0] # placeholder
-        R.files += [f for f in inFiles if not isinstance(f,str)] # in case passing bytes or JSON directly
+        R.files = inFiles # may mix dict + string, even in same category especially if using "skip", so don't separate types
     else: # being called from the command line
         R.__dict__.update(get_argument_parser().parse_args().__dict__)
     R.__dict__.update((k,v)
                       for k,v in kwargs.items()
                       if type(v) not in [str,int,type(None)]) # (None means keep the default from parse_args; boolean and bytes we might as well handle directly; list e.g. merge_books should bypass parser; ditto session object for cache, a type we can't even name here if requests_cache is not installed)
     for k in ['merge_books','chapter_titles']:
         if not isinstance(R.__dict__[k],list):
@@ -272,15 +270,17 @@
     for f in R.files:
         fOrig = f
         if isinstance(f,dict):
             # support direct JSON pass-in as dict
             R.jsonData.append(f)
             R.check_for_JSON_transcript()
             continue
-        if isinstance(f,str) and f.lower().endswith(f"{os.extsep}zip"):
+        elif f=="skip": # we're 'full text some audio' and we're skipping audio for a chapter
+            R.jsonData.append(None) ; continue
+        elif isinstance(f,str) and f.lower().endswith(f"{os.extsep}zip"):
             if R.outputFile: error(f"Only one {os.extsep}zip output file may be specified")
             R.outputFile = f ; continue
         elif isinstance(f,str) and re.match("https?://",f):
             f=fetch(f,R.cache,R.refresh,R.refetch,R.delay,R.user_agent)
         elif delimited(f,'{','}'): pass
         elif delimited(f,'<','>'): pass
         elif not os.path.isfile(f): error(f"File not found: {f}")
@@ -292,29 +292,41 @@
             R.htmlData.append(f)
         elif fOrig.lower().endswith(f"{os.extsep}mp3") or fOrig.lower().endswith(f"{os.extsep}wav"):
             R.audioData.append(f)
             R.filenameTitles.append(fOrig[:fOrig.rindex(os.extsep)])
         elif fOrig.lower().endswith(f"{os.extsep}txt"):
             R.textData.append(f.decode('utf-8').strip())
         else: error(f"Format of '{fOrig}' has not been recognised")
+    if R.htmlData: # check for text-only DAISY:
+        if not R.jsonData:
+            R.jsonData=[None]*len(R.htmlData)
+        if not R.audioData:
+            R.audioData=[None]*len(R.htmlData)
+    # and check for full-text part-audio DAISY:
+    if len(R.jsonData) > len(R.audioData):
+        for c,i in enumerate(R.jsonData):
+            if i is None:
+                R.audioData.insert(c,None)
+    if not R.outputFile:
+        R.outputFile=f"output_daisy{os.extsep}zip"
+    if not R.title: R.title=R.outputFile.replace(f"{os.extsep}zip","").replace("_daisy","")
   def check(self) -> None:
-    "Checks we've got everything"
-    # You may omit calling this if you're creating
-    # a temporary Run just to call something like
-    # check_for_JSON_transcript and get its HTML
+    """Checks we've got everything.
+    You may omit calling this if you're creating
+    a temporary Run just to call something like
+    check_for_JSON_transcript and get its HTML."""
     R = self
-    if R.htmlData and R.audioData and not R.jsonData: error("Full text and audio without time markers is not yet implemented")
+    if R.htmlData and any(a and not j for a,j in zip(R.audioData,R.jsonData)): error("Full text and audio without time markers is not yet implemented")
     if R.jsonData and not R.htmlData: error("Time markers without full text is not implemented")
     if R.htmlData and R.textData: error("Combining full text with title-only text files is not yet implemented.  Please specify full text for everything or just titles for everything, not both.")
     if R.jsonData and not len(R.audioData)==len(R.jsonData): error(f"If JSON marker files are specified, there must be exactly one JSON file for each recording file.  We got f{len(R.jsonData)} JSON files and f{len(R.audioData)} recording files.")
     if R.textData and not len(R.audioData)==len(R.textData): error(f"If text files are specified, there must be exactly one text file for each recording file.  We got f{len(R.textData)} text files and f{len(R.audioData)} recording files.")
-    if R.htmlData and R.audioData and not len(R.audioData)==len(R.htmlData): error(f"If HTML documents with audio are specified, there must be exactly one HTML document for each recording.  We got f{len(R.htmlData)} HTML documents and f{len(R.audioData)} recordings.")
-    if not R.outputFile:
-        R.outputFile=f"output_daisy{os.extsep}zip"
-    if not R.title: R.title=R.outputFile.replace(f"{os.extsep}zip","").replace("_daisy","")
+    if R.htmlData and not len(R.audioData)==len(R.htmlData): error(f"If HTML documents with audio are specified, there must be exactly one HTML document for each recording.  We got f{len(R.htmlData)} HTML documents and f{len(R.audioData)} recordings.")
+    if R.htmlData and not len(R.htmlData)==len(dict.fromkeys(R.htmlData).keys()): error("Duplicate HTML input documents")
+    if not R.htmlData and not R.textData and not R.audioData: error("No input given")
   def warning(self,warningText) -> None:
     if self.warnings_are_errors:error(warningText)
     self.warnings.append(warningText)
     sys.stderr.write(f"WARNING: {warningText}\n")
   def check_for_JSON_transcript(self) -> None:
     """Checks to see if the last thing added to
     the Run object is a JSON podcast transcript,
@@ -336,41 +348,43 @@
         R.htmlData.append(' '.join(
             f'<span {R.marker_attribute}="{i}">{c}</span>' for i,c in enumerate(bodyList) if c))
         R.jsonData[-1]={"markers":[
             {"id":f"{i}","time":t}
             for i,t in enumerate(
                     s["startTime"] for s in R.jsonData[-1]["segments"])
             if bodyList[i]]}
-  def make_null_jsonData(self) -> None:
+  def get_null_jsonData(self,h) -> dict:
     """Generate no-audio JSON for internal use
     when making text-only DAISY files from HTML.
     In this case we assume any element with any
     marker-attribute should be extracted."""
-    self.jsonData = [
-        {'markers':
-         [{'id':i[self.marker_attribute], 'time':0}
+    return {'markers':
+         [{'id':i[self.marker_attribute],'time':0}
           for i in BeautifulSoup(h,'html.parser')
           .find_all(**{self.marker_attribute:
                        True})]}
-        for h in self.htmlData]
   def get_texts(self) -> list:
     """Gets the text markup required for the run,
     extracting it from HTML (guided by JSON IDs)
     if we need to do that."""
     R = self
     if R.textData: return R.textData # section titles only, from text files
     elif not R.htmlData: return R.filenameTitles # section titles only, from sound filenames
-    elif not R.jsonData: self.make_null_jsonData()
     recordingTexts = []
     for h,j in zip(R.htmlData,R.jsonData):
+        if j is None:
+            j = R.get_null_jsonData(h)
+            include_alt_tags_in_text = True
+        else: include_alt_tags_in_text = False # because we won't be able to match it up to the audio
         markers = j['markers']
         want_pids = [jsonAttr(m,"id") for m in markers]
         extractor = PidsExtractor(R,want_pids)
         extractor.handle_soup(
-            BeautifulSoup(h, 'html.parser'))
+            BeautifulSoup(h, 'html.parser'),
+            include_alt=include_alt_tags_in_text)
         rTxt = []
         for i in range(len(markers)):
             rTxt.append(parseTime(jsonAttr(markers[i],"time")))
             if want_pids[i] in extractor.id_to_content:
                 tag,content = extractor.id_to_content[want_pids[i]]
                 content = ''.join(content).strip()
                 rTxt.append(TagAndText(tag,content_fixes(content)))
@@ -383,30 +397,32 @@
   def write_all(self,recordingTexts) -> None:
     """Writes the DAISY zip and everything in it.
     Each item of recordingTexts is either 1 text
     for section title of whole recording, or a
     TextsAndTimesWithPages i.e. ([TagAndText,time,
     TagAndText,time,TagAndText],[PageInfo,...])"""
     R = self
-    assert len(R.audioData) == len(recordingTexts) or not R.audioData
+    assert len(R.audioData) == len(recordingTexts)
+    assert recordingTexts
     headings = R.getHeadings(recordingTexts)
     if R.dry_run: return sys.stderr.write(f"Dry run: {len(R.warnings) if R.warnings else 'no'} warning{'' if len(R.warnings)==1 else 's'} for {R.outputFile}\n")
-    if R.audioData: merge0lenSpans(recordingTexts,headings)
-    if R.mp3_recode and R.audioData or any(
-            'audio/mp3' not in mutagen.File(BytesIO(dat)).mime for dat in R.audioData): # parallelise lame if possible
+    merge0lenSpans(recordingTexts,headings,R.audioData)
+    if R.mp3_recode and any(R.audioData) or any(
+            'audio/mp3' not in mutagen.File(BytesIO(dat)).mime for dat in R.audioData if dat): # parallelise lame if possible
         if not __name__=="__main__":
             sys.stderr.write(f"Making {R.outputFile}...\n"),sys.stderr.flush() # especially if repeatedly called, print which outputFile we're working on BEFORE the mp3s also
         executor = ThreadPoolExecutor(
             max_workers=cpu_count())
-        recordingTasks=[executor.submit(
+        recordingTasks=[(executor.submit(
             (recodeMP3 if
              R.mp3_recode or
              'audio/mp3' not in mutagen.File(BytesIO(dat)).mime
              else lambda x:x),
-            dat) for dat in R.audioData]
+            dat) if dat else None)
+                        for dat in R.audioData]
     else: executor,recordingTasks = None,None
     try: R.write_all0(recordingTexts,headings,recordingTasks)
     except: # unhandled exception: clean up
         try: executor.shutdown(wait=False,cancel_futures=False) # (cancel_futures is Python 3.9+)
         except: pass # (no executor / can't do it) # noqa: E722
         try: os.remove(R.outputFile) # incomplete
         except: pass # noqa: E722
@@ -452,26 +468,26 @@
     # (it's iOS users that need the above, apparently.  Can't DAISY have a non-ZIP extension so Apple systems don't automatically unpack it?  but we do need to manually unpack if writing to a CD-ROM for old devices.  Can't Apple look at some kind of embedded "don't auto-unpack this zip" request?)
     secsSoFar = 0
     durations = [] ; curP = 1
     for recNo in range(1,len(recordingTexts)+1):
         rTxt = recordingTexts[recNo-1]
         secsThisRecording = mutagen.File(
             BytesIO(R.audioData[recNo-1])
-        ).info.length if R.audioData else 0
+        ).info.length if R.audioData[recNo-1] else 0
         if secsThisRecording > 3600: R.warning(f"Recording {recNo} is long enough to cause ~{secsThisRecording*.0001:.1f}sec synchronisation error on some readers") # seems lame v3.100 can result in timestamps being effectively multiplied by ~1.0001 on some players but not all, causing slight de-sync on 1h+ recordings (bladeenc may avoid this but be lower quality overall; better to keep the recordings shorter if possible)
         durations.append(secsThisRecording)
-        if recordingTasks is not None:
-            sys.stderr.write(f"Adding {recNo:04d}.mp3..."),sys.stderr.flush()
-        if R.audioData:
+        if R.audioData[recNo-1]:
+            if recordingTasks is not None:
+                sys.stderr.write(f"Adding {recNo:04d}.mp3..."),sys.stderr.flush()
             writestr(f"{recNo:04d}.mp3",
                  R.audioData[recNo-1]
                  if recordingTasks is None
                  else recordingTasks[recNo-1].result())
-        if recordingTasks is not None:
-            sys.stderr.write(" done\n")
+            if recordingTasks is not None:
+                sys.stderr.write(" done\n")
         writestr(f'{recNo:04d}.smil',D(
             R.section_smil(recNo,secsSoFar,
                          secsThisRecording,curP,
                          rTxt.textsAndTimes if isinstance(rTxt,TextsAndTimesWithPages) else rTxt)))
         writestr(f'{recNo:04d}.{"xml" if R.daisy3 else "htm"}',
                  D(R.text_htm(
                      (rTxt.textsAndTimes[
@@ -537,15 +553,15 @@
             if not tag.startswith('h'):
                 continue
             if v//2 - 1 == first//2 and not textsAndTimes[first].tag.startswith('h'): # chapter starts with non-heading followed by heading: check the non-heading for "Chapter N" etc
                 nums=re.findall("[1-9][0-9]*",textsAndTimes[first].text)
                 if len(nums)==1:
                     text=f"{nums[0]}: {text}" # for TOC
                     textsAndTimes[v-1] = (textsAndTimes[first-1] if first else 0) + 0.001 # for audio jump-navigation to include the "Chapter N" (TODO: option to merge the in-chapter text instead, so "Chapter N" appears as part of the heading, not scrolled past quickly?  merge0lenSpans will now do this if the chapter paragraph is promoted to heading, but beware we might not want the whole of the 'chapter N' text to be part of the TOC, just the number.  Thorium actually stops playing when it hits the 0-length paragraph before the heading, so promoting it might be better; trying the +0.001 for now to make timestamps not exactly equal)
-            chapHeadings.append(ChapterTOCInfo(tag,re.sub('<img src.*?/>','',text),v//2))
+            chapHeadings.append(ChapterTOCInfo(tag,re.sub('<[^>]*>','',text),v//2))
         if not chapHeadings:
             # This'll be a problem, as master_smil and ncc_html need headings to refer to the chapter at all.  (Well, ncc_html can also do it by page number if we have them, but we haven't tested all DAISY readers with page number only navigation, and what if we don't even have page numbers?)
             # So let's see if we can at least get a chapter number.
             if first is not None: nums=re.findall("[1-9][0-9]*",textsAndTimes[first].text)
             else:
                 R.warning(f"Chapter {chapNo} is completely blank!  (Is {'--marker-attribute' if __name__=='__main__' else 'marker_attribute'} set correctly?)")
                 nums = [] ; first = 0 ; textsAndTimes.append(TagAndText('p',''))
@@ -672,23 +688,26 @@
     <meta name="ncc:pageFront" content="0" />
     <meta name="ncc:maxPageNormal" content="{maxPageNo}" />
     <meta name="ncc:pageNormal" content="{numPages}" />
     <meta name="ncc:pageSpecial" content="0" />
     <meta name="ncc:tocItems" content="{len(headingsR)+sum(len(PNs) for PNs in pageNos)}" />
     <meta name="ncc:totalTime" content="{hmsTime(totalSecs)}" />
     <meta name="ncc:multimediaType" content="{
-    "textNcc" if not R.audioData else
+    "textNcc" if not any(R.audioData) else
+    "textPartAudio" if hasFullText and not all(R.audioData) else
     "audioFullText" if hasFullText else "audioNcc" }" />
     <meta name="{'dtb' if R.daisy3 else 'ncc'
     }:depth" content="{max(int(h.hTag[1:])
     for h in headingsR if h.hTag.startswith('h'))
     +(1 if any(h.hTag=='div' for h in headingsR)
     else 0)}" />
-    <meta name="ncc:files" content="{2+
-    len(headings)*(3 if hasFullText and R.audioData else 2)+len(R.imageFiles)}" />
+    <meta name="ncc:files" content="{ 2
+    + sum(1 for a in R.audioData if a)
+    + len(headings)*(2 if hasFullText else 1)
+    + len(R.imageFiles)}" />
   </head>
   {f'<docTitle><text>{R.title}</text></docTitle>'
     if R.daisy3 else ''}
   {f'<docAuthor><text>{R.creator}</text></docAuthor>'
     if R.daisy3 else ''}
   <{'navMap id="navMap"' if R.daisy3 else 'body'}>"""+''.join((f"""
     <navPoint id="s{s+1}" class="{t.hTag}" playOrder="{s+1}">
@@ -962,98 +981,110 @@
     </{'bodymatter></book' if R.daisy3 else 'body'}>
 </{'dtbook' if R.daisy3 else 'html'}>
 """)
 
 class PidsExtractor:
     """Go through the HTML, extracting the
     paragraphs whose IDs we want, and moving any
-    images between two ID'd paragraphs to the
-    previously-ID'd paragraph, discarding others
-    (site decoration etc).  Also pick up on any
-    page-number tags and note where they were."""
+    images to their relevant ID'd paragraph (we
+    assume all images with an image_attribute
+    should be kept, and others are site decoration
+    etc).  Also pick up on any page-number tags
+    and note where they were."""
     
     def __init__(self, R:Run, want_pids:list[str]):
         self.R = R
         self.want_pids = want_pids # IDs we want
         self.id_to_content = {} # our main output
         self.pageNos = [] # secondary output for page-number based navigation
         self.pageNoGoesAfter = 0 # want_pids index
         self.previous_pid_tagname = None
         self.previous_pid_contents = None
-        self.images_since_previous_pid_closed = []
+        self.images_before_first_pid = []
+        self.seen_heading = False
     
-    def handle_soup(self,t,addTo=None) -> None:
+    def handle_soup(self,t,addTo=None,
+                    include_alt=False) -> None:
         """Recursively scan through the HTML.
         t is a BeautifulSoup tree node.
         addTo is the list of data for the ID that
         is currently being extracted, if any: we
-        can append to this."""
+        can append to this.
+        include_alt is True if we want to repeat
+        the ALT tags of included images in text"""
         
         if not t.name: # data or comment
             if t.PREFIX: pass # ignore comment, doctype etc
             elif addTo is not None: # collect text
                 addTo.append(str(t).replace('&','&amp;').replace('<','&lt;'))
             return
         # ok, it's a tag:
         tag=tagRewrite.get(t.name,t.name)
         attrs = t.attrs
         imgURL = attrs.get(self.R.image_attribute,None)
         if imgURL and (re.match(
                 "https?://.*[.][^/]*$",
-                imgURL) or os.path.isfile(
-                    imgURL)) and not (
-                        addTo is None
-                        and self.previous_pid_contents is None):
+                imgURL)or os.path.isfile(imgURL)):
             # Write the 'img' markup for the DAISY document.
             # Will be moved to after the paragraph by text_htm
             # because DAISY images cannot occur inside paragraphs.
-            # (Might want to check attrs.get("alt",""), but DAISY3 standard does not list alt as a valid attribute for img, so we'd have to put it after with br etc (changing text_htm) and we don't know if it's in the audio or not: probably best just to leave it and rely on there being a separate caption with ID if it's in the audio)
             image_index = self.R.imageFiles.index(imgURL) if imgURL in self.R.imageFiles else len(self.R.imageFiles)
             img = f'''<img src="{
             image_index+1}{
             imgURL[imgURL.rindex("."):]
             }" {f'id="i{image_index}"'
             if self.R.daisy3 else ""} />'''
             if imgURL not in self.R.imageFiles:
                 self.R.imageFiles.append(imgURL)
-            if addTo is not None:
-                addTo.append(img)
-            else: self.images_since_previous_pid_closed.append(img) # in case we get another paragraph
+            if "alt" not in attrs:
+                for k in attrs.keys():
+                    if k.endswith("-alt"): # data-img-att-alt or whatever (TODO: customisable?)
+                        attrs["alt"] = attrs[k]
+                        break
+            if include_alt and "alt" in attrs:
+                # DAISY3 standard does not list alt as a valid attribute for img, so we have to put the text in afterwards
+                img += f'<br>{attrs["alt"]}<br>' # images will be moved to *after* these by text_htm; if we want an option for the image *before* the ALT, we'd need to put these in the *next* paragraph or change text_htm
+            if addTo is not None:addTo.append(img)
+            elif self.previous_pid_contents is not None: self.previous_pid_contents.append(img)
+            else: self.images_before_first_pid.append(img)
         this_tag_has_a_pid_we_want = False
         if attrs.get(self.R.marker_attribute,None) in self.want_pids:
             this_tag_has_a_pid_we_want = True
             self.previous_pid_tagname = tag
             a = attrs[self.R.marker_attribute]
             self.pageNoGoesAfter = self.want_pids.index(a)
             self.id_to_content[a] = ((tag if re.match('h[1-6]$',tag) or tag=='span' else 'p'),[])
-            if self.images_since_previous_pid_closed:
-                self.previous_pid_contents += self.images_since_previous_pid_closed
-                self.images_since_previous_pid_closed = []
             addTo = self.id_to_content[a][1]
         elif addTo is not None and tag in allowedInlineTags: addTo.append(f'<{allowedInlineTags[tag]}>')
         elif addTo is not None and tag=='a': self.lastAStart = len(addTo)
         pageNo = attrs.get(self.R.page_attribute,None)
         if pageNo: self.pageNos.append(PageInfo(self.pageNoGoesAfter,pageNo))
         # Now the recursive call:
         if not tag=='rt':
           for c in t.children:
-            self.handle_soup(c,addTo)
+            self.handle_soup(c,addTo,include_alt)
         # And now the end tag:
         if addTo is not None:
             if this_tag_has_a_pid_we_want:
-                self.highestImage,self.previous_pid_contents = len(self.R.imageFiles),addTo
+                self.seen_heading = tag.startswith("h")
+                if self.images_before_first_pid and self.seen_heading and not (
+                        tag.startswith("h")
+                        and any("<br" in i
+                            for i in self.images_before_first_pid)): # (don't include ALTs as part of the heading, and ALT or otherwise don't risk putting before first heading especially if we'll rewrite number to be part of it)
+                    addTo += self.images_before_first_pid
+                    self.images_before_first_pid=None
+                self.previous_pid_contents = addTo
             elif tag in allowedInlineTags: addTo.append(f'</{allowedInlineTags[tag]}>')
             elif tag=="a" and re.match('[!-.:-~]$',"".join(addTo[self.lastAStart:]).strip()):
                 # remove single-character link, probably to footnote (we won't know if it's in the audio or not, we're not supporting jumps and the symbols might need normalising)
                 # but don't remove numbers (might be paragraph numbers etc) or non-ASCII (might be single-character CJK word)
                 del addTo[self.lastAStart:]
         elif tag=='p' and self.previous_pid_contents and self.previous_pid_tagname=='span':
             # if paragraphs contain spans and it's the spans that are identified, ensure we keep this break in the surrounding structure
             self.previous_pid_contents.append("<br>")
-        if tag=='html' and self.images_since_previous_pid_closed and hasattr(self,'highestImage'): del self.R.imageFiles[self.highestImage:] # do not include ones that are still only in images_since_previous_pid_closed at the end of the page (and not also elsewhere)
 
 def delimited(s,start:int,end:int) -> bool:
     """Checks to see if a string or binary data
     is delimited by start and end, converting as
     needed, after stripping"""
     if isinstance(s,bytes):
         s = s.replace(b"\xEF\xBB\xBF",b"").strip() # just in case somebody's using UTF-8 BOMs
@@ -1132,28 +1163,28 @@
     and returns floating-point seconds"""
     
     tot = 0.0 ; mul = 1
     for u in reversed(t.split(':')):
         tot += float(u)*mul ; mul *= 60
     return tot
 
-def merge0lenSpans(recordingTexts:list, headings:list) -> None:
+def merge0lenSpans(recordingTexts:list, headings:list, hasAudio:list) -> None:
     """Finds spans in the text that are marked as
     zero length in the audio, and merges them into
     their neighbours if possible.  This is so that
     the resulting DAISY file can still be
     navigable if some of the time markers are
     somehow missing in the input JSON, i.e. we
     don't know when item 1 becomes item 2, but we
     do know where item 1 starts and where item 2
     ends, so can we set the navigation to create
     a combined item for both 1 and 2."""
     
-    for cT,cH in zip(recordingTexts,headings):
-        if not isinstance(cT,TextsAndTimesWithPages): continue
+    for cT,cH,hA in zip(recordingTexts,headings,hasAudio):
+        if not hA or not isinstance(cT,TextsAndTimesWithPages): continue
         textsAndTimes,pages = cT
         i=0
         while i < len(textsAndTimes)-2:
             while i < len(textsAndTimes)-2 and \
                   isinstance(textsAndTimes[i],TagAndText) and \
             (0 if i==0 else textsAndTimes[i-1])==\
             textsAndTimes[i+1] and \
@@ -1251,15 +1282,18 @@
     try: _last_urlopen_time
     except NameError: _last_urlopen_time = 0
     if delay: time.sleep(min(0,_last_urlopen_time+delay-time.time()))
     headers = {"User-Agent":user_agent} if user_agent else {}
     if ifModSince:
         t = time.gmtime(ifModSince)
         headers["If-Modified-Since"]=f"{'Mon Tue Wed Thu Fri Sat Sun'.split()[t.tm_wday]}, {t.tm_mday} {'Jan Feb Mar Apr May Jun Jul Aug Sep Oct Nov Dec'.split()[t.tm_mon-1]} {t.tm_year} {t.tm_hour:02d}:{t.tm_min:02d}:{t.tm_sec:02d} GMT"
-    try: dat = urlopen(Request(url,headers=headers)).read()
+    url2 = ''.join(
+        (chr(b) if b < 128 else f"%{b:02x}")
+        for b in url.encode('utf-8'))
+    try: dat = urlopen(Request(url2,headers=headers)).read()
     except HTTPError as e:
         _last_urlopen_time = time.time()
         if e.getcode()==304 and cache:
             sys.stderr.write(" no new data\n")
             return open(fn,'rb').read()
         else:
             sys.stderr.write(f"error {e.getcode()}\n")
@@ -1310,15 +1344,15 @@
         ('' if not i.hTag.startswith('h')
          else i.hTag[1]
          if int(i.hTag[1])>=nextDepth
          else '0')
         for i in reversed(headingsR[:s+1])
     ).split('0',1)[0]
     if thisDepth: D=thisDepth
-    else: D=int(headingNums_closed[0]) # the heading before this div (TODO: this code assumes there will be one, which is currently true as these divs are generated only by verse numbering)
+    else: D=int(headingNums_closed[0]) # the heading before this div (this code assumes there will be one, which is currently true as these divs are generated only by verse numbering)
     N = sum(1 for j in range(nextDepth,D+1)
             if str(j) in headingNums_closed)
     return N+(1 if thisDepth is None else 0)
 
 def hReduce(headings:list) -> list[BookTOCInfo]:
     """convert a list of ChapterTOCInfo lists (or
     text strings for unstructured chapters) into a
```

### Comparing `anemone_daisy_maker-1.59/anemone_daisy_maker.egg-info/PKG-INFO` & `anemone_daisy_maker-1.60/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: anemone-daisy-maker
-Version: 1.59
+Name: anemone_daisy_maker
+Version: 1.60
 Summary: Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data
 Home-page: http://ssb22.user.srcf.net/indexer/anemone.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -14,22 +14,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
-`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce three different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It can produce four different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
 3. Text with no audio: this requires just XHTML files, and extracts all text with a specified attribute (`data-pid` by default)
 
+4. Text with some audio: this is a combination of the above two methods, and you'll need to specify `skip` in the JSON file list for the chapters that do not yet have recorded audio
+
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
 ### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
```

### Comparing `anemone_daisy_maker-1.59/setup.py` & `anemone_daisy_maker-1.60/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.59',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='any',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
+from setuptools import setup, find_packages;setup(name='anemone_daisy_maker',version='1.60',entry_points={'console_scripts':['anemone=anemone.__init__:anemone']},license='Apache 2',platforms='any',url='http://ssb22.user.srcf.net/indexer/anemone.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Create DAISY digital talking books from HTML text, MP3 audio and JSON time index data',long_description='''Anemone DAISY maker
 -----------------
 from http://ssb22.user.srcf.net/indexer/anemone.html
 
-`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It currently can produce three different types of digital talking book:
+`anemone.py` is a module to put together a DAISY digital talking book, from HTML text, MP3 audio recordings and time index data.  It produces DAISY 2.02 files by default, or DAISY 3 (i.e. ANSI/NISO Z39.86) if an option is set.  It can produce four different types of digital talking book:
 
 1. Full audio with basic Navigation Control Centre only: this requires a list of MP3 or WAV files for the audio, one per section, and the title of each section can be placed either in a separate text file or in the filename of the audio file.
 
 2. Full audio with full text: this requires MP3 or WAV files for the audio, corresponding XHTML files for the text, and corresponding JSON files for the timing synchronisation.  Each JSON file is expected to contain a list called `"markers"` whose items contain `"id"` (or `"paragraphId"` or anything else ending id) and `"time"` (or `"startTime"` or anything else ending time), which can be in seconds, minutes:seconds or hours:minutes:seconds (fractions of a second are allowed in each case).  The IDs in these JSON files should have corresponding attributes in the XHTML, by default data-pid but this can be changed with an option.
 
 3. Text with no audio: this requires just XHTML files, and extracts all text with a specified attribute (`data-pid` by default)
 
+4. Text with some audio: this is a combination of the above two methods, and you'll need to specify `skip` in the JSON file list for the chapters that do not yet have recorded audio
+
 All files are placed on the command line (or in parameters if you're using Anemone as a module), and Anemone assumes the correspondences are ordered.  So for example if MP3, HTML and JSON files are given, Anemone assumes the first-listed MP3 file corresponds with the first-listed HTML file and the first-listed JSON file, and so on for the second, third, etc.  With most sensible file naming schemes, you should be able to use shell wildcards like `*` when passing the files to Anemone.  You may also set the name of an output file ending `zip`; the suffix `_daisy.zip` is common.  The title, publisher, language etc of the book should be set via options: run the program with `--help` to see all.
 
 The daisy anemone is a sea creature on the rocky Western shores of Britain and Ireland; the Dorset Wildlife Trust says it's "usually found in deep pools or hiding in holes or crevices, or buried in the sediment with only tentacles displayed".  Similarly this script has no interactive user interface; it hides away on the command line, or as a library module for your Python program.
 
 ### Behaviour of DAISY readers in 2024
 
 * Dolphin EasyReader 10 (iOS, Android and Chromebook): is able to open the ZIP and play the audio while highlighting the paragraphs in a ‘full audio plus full text’ book, both Daisy 2 and Daisy 3.  In very large books (over 1&nbsp;GB), loading and navigation becomes unreliable.
```

