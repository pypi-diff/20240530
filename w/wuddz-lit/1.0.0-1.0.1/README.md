# Comparing `tmp/wuddz_lit-1.0.0.tar.gz` & `tmp/wuddz_lit-1.0.1.tar.gz`

## Comparing `wuddz_lit-1.0.0.tar` & `wuddz_lit-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 wuddz_lit-1.0.0/wuddz_lit/lit.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 wuddz_lit-1.0.0/LICENSE
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 wuddz_lit-1.0.0/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wuddz_lit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 wuddz_lit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    19691 2020-02-02 00:00:00.000000 wuddz_lit-1.0.1/wuddz_lit/lit.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 wuddz_lit-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 wuddz_lit-1.0.1/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 wuddz_lit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 wuddz_lit-1.0.1/PKG-INFO
```

### Comparing `wuddz_lit-1.0.0/wuddz_lit/lit.py` & `wuddz_lit-1.0.1/wuddz_lit/lit.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,18 +146,18 @@
                 ic = int(ai['last_page'])  #Amount Of Pages (50 Stories Per Page) Containing All Author Stories
                 a = ai['data'][0]['authorname']
                 dr = self.gdir(a) if self.args.download else ''
                 with open(path.join(self.lout, f'{a}.txt'), 'w', encoding='utf-8') as fw:
                     for i in range(1, ic + 1):  #Iterate Total Pages Of Author Stories
                         if i > 1:
                             ai = self.resp(url+"?params={%22page%22:%20"+str(i)+"}").json()  #Subsequent Paginated Author API Responses
-                        for i in range(len(ai['data'])):  #Iterate API Json Response Containing Story Data Per Page
+                        for n in range(len(ai['data'])):  #Iterate API Json Response Containing Story Data Per Page
                             self.gl += 1
-                            t = ai['data'][i]['url']  #Story Title
-                            c = ai['data'][i]['category_info']['pageUrl']  #Story Category
+                            t = ai['data'][n]['url']  #Story Title
+                            c = ai['data'][n]['category_info']['pageUrl']  #Story Category
                             sl.append(t)
                             fw.write(t+' '+'_'*(71-len(t))+c+'\n')  #Write Story Titles & Matching Categories To Output File
         return [sl,dr]
     
     def category(self, c: str, u: str) -> list:
         """
         Returns A List Containing A List Of Specified Category Stories & Output Directory Path.
@@ -206,44 +206,50 @@
             aut = js['submission']['authorname']  #Story Author Name
             cat = js['submission']['category_info']['pageUrl']  #Story Category
             tit = js['submission']['title']  #Story Title
             typ = js['submission']['type']  #Story Type
             if cat in self.nto and self.args.text:return
             dr = self.gdir(path.join(dr, st))
             for i in range(1, pgs+1):  #Iterate Story Pages
-                fn = path.join(dr, f'{st}__Page')
+                fn = path.join(dr, f'{st}__Page{i}.html')
+                txt = ''
                 if i > 1:
                     uri = surl+"?params={%22contentPage%22:%20"+str(i)+"}"
                     js = self.resp(uri).json()
-                if self.args.text and js.get('pageText'):
-                    sc += 1
-                    txt = js['pageText']
-                    self.text(txt, f'{fn}{i}.txt', (aut,cat,dsc,tit,uid))
-                elif not self.args.text:
-                    txt = ''
-                    if typ == 'illustra':txt = self.art(st, dr, js)
+                if js.get('pageText'):
+                    if self.args.text:
+                        sc += 1
+                        fn = f'{fn[:-4]}txt'
+                        tt = self.text(js['pageText'])
+                        rem = re.compile('<.*?>')
+                        tt = re.sub(rem, '', tt)
+                        tt = tt.replace('    ', '')
+                        txt = "Title: %s\nAuthor: %s\nUser_Id: %s\nCategory: %s\nDescription: %s\n\n%s" %(tit,aut,uid,cat,dsc,tt)
                     else:
-                        url = self.hurl %(st)
-                        if 'poetry' in cat:url = self.purl %(st)
-                        if i > 1:url = f'{url}?page={i}'
-                        txt = self.resp(url).text
-                        if typ == 'audio':txt = self.audio(st, txt, fn.split('__')[0])
-                        elif cat in ['illustrated-erotic-fiction', 'illustrated-poetry']:
-                            txt = self.illus(txt, dr)
+                        if typ == 'illustra':txt = self.art(st, dr, js)
+                        else:
+                            url = self.hurl %(st)
+                            if 'poetry' in cat:url = self.purl %(st)
+                            if i > 1:url = f'{url}?page={i}'
+                            txt = self.resp(url).text
+                            if typ == 'audio':txt = self.audio(st, txt, fn.split('__')[0])
+                            elif cat in ['illustrated-erotic-fiction', 'illustrated-poetry']:
+                                txt = self.illus(txt, dr)
+                        if txt:
+                            sc += 1
+                            if pgs > 1:
+                                if not ht:
+                                    ht = re.search(r'href="(/\w/'+st+'\?page=)\d+"', txt).group(1)
+                                    ft = ht.split('?')[0]
+                                # Link Locally Saved Html Pages For Easy Navigation
+                                for n in range(2, pgs+1):
+                                    txt = txt.replace(f'{ht}{n}', f'./{st}__Page{n}.html')
+                                txt = txt.replace(ft, f'./{st}__Page1.html')
                     if txt:
-                        sc += 1
-                        if pgs > 1:
-                            if not ht:
-                                ht = re.search(r'href="(/\w/'+st+'\?page=)\d+"', txt).group(1)
-                                ft = ht.split('?')[0]
-                            # Link Locally Saved Html Pages For Easy Navigation
-                            for n in range(2, pgs+1):
-                                txt = txt.replace(f'{ht}{n}', f'./{st}__Page{n}.html')
-                            txt = txt.replace(ft, f'./{st}__Page1.html')
-                        with open(f'{fn}{i}.html', 'w', encoding='utf-8') as fw:
+                        with open(fn, 'w', encoding='utf-8') as fw:
                             fw.write(txt)
         if sc != 0:self.gs += 1
     
     def audio(self, st: str, txt: str, fn: str) -> str:
         """
         Downloads Audio Story With Media File(s) & Returns Locally Linked Html Output.
         :param st: String Audio Story Title.
@@ -274,25 +280,22 @@
             self.dfile(irl, ifn)
             #Replace Image Url(s) With Downloaded Image Path(s) In Story Html.
             tt = tt.replace('<img src="%s"' %(rrl), '</div><img src="%s"' %(f'./{i}.{ext}'))
         
         #Return Edited Art Story Html Containing Image File(s) Linked Locally For Offline Viewing.
         return tt
     
-    def text(self, fa: str, fn: str, io: tuple):
+    def text(self, fa: str, wv: int=128):
+        """
+        Returns TextWrap Formatted Story Text With Default Width (128 chars) Or Specified Width.
+        :param fa: String Story Text To Be Formatted.
+        :param wv: Integer Value Of Width To Format Text Default=128.
         """
-        Writes Formatted Story Text Output To File.
-        :param fa: String Story Text.
-        :param fn: String Filename To Save Story Output.
-        :param io: Tuple Containing Info To Be Written To Story Output.
-        """
-        wc = textwrap.TextWrapper(width=128)  #Awesome Textwrap TextWrapper Class To Output Text 128 Characters Per Line
-        tw = wc.fill(text=fa)
-        with open(fn, 'w', encoding='utf-8') as fw:
-            fw.write(f"Title: {io[3]}\nAuthor: {io[0]}\nUser_Id: {io[4]}\nCategory: {io[1]}\nDescription: {io[2]}\n\n{tw}")
+        wc = textwrap.TextWrapper(width=wv)  #Awesome Textwrap TextWrapper Class To Output Text 128 Characters Per Line
+        return wc.fill(text=fa)
     
     def mlist(self, e, l: list, u: str = None) -> list:
         """
         Returns Retrieved Author/Category Stories As List.
         :param e: Class Concurrent Futures ThreadPoolExecutor Instance.
         :param l: List Of Specified Authors/Categories To Retrieve Stories For.
         :param u: String Specifying Category Stories To Be Retrieved (Default = None (i.e Author Stories)).
@@ -323,17 +326,17 @@
                 if dl:ml = self.mlist(ex, dl, u='c')  #Retrieve & List Category Stories
             elif self.args.story:ml = [[dl, self.gdir('Misc')]]
             if self.args.download and ml:
                 #Iterate & Download Stories With Concurrent.Futures ThreadPoolExecutor Threads
                 for m in ml:
                     for i in m[0]:
                         ex.submit(self.story(i, m[1]))
-            if self.gs > 0:print(f'\n{self.gs} Stories Downloaded To Respective Folders In {self.sout}')
-            elif self.gl > 0:print(f'\n{self.gl} Stories Listed To Text File(s) In {self.lout}')
-            else:print('\nNo Stories Listed Or Downloaded Enter Valid Arguments Or Check Internet Connection!!')
+        if self.gs > 0:print(f'\n{self.gs} Stories Downloaded To Respective Folders In {self.sout}')
+        elif self.gl > 0:print(f'\n{self.gl} Stories Listed To Text File(s) In {self.lout}')
+        else:print('\nNo Stories Listed Or Downloaded Enter Valid Arguments Or Check Internet Connection!!')
 
 def cli_main():
     """
     Wuddz-Lit Entry Point Executing Specified Argparse NameSpace Arguments.
     """
     usage = ('[*]EXAMPLES:\n'
              '  wudz-lit -f "C:\\file.txt" -s -d -x 100   Download Stories In "C:\\file.txt" File As Html Using 100 Threads.\n'
```

### Comparing `wuddz_lit-1.0.0/LICENSE` & `wuddz_lit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wuddz_lit-1.0.0/README.md` & `wuddz_lit-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ## Installation
 Install using [PyPI](https://pypi.org/project/wuddz-lit):
 ```
 pip install wuddz-lit
 ```
 Install locally by cloning or downloading and extracting the repo, then cd into 'dist' directory and execute:
 ```
-pip install wuddz_lit-1.0.0.tar.gz
+pip install wuddz_lit-1.0.1.tar.gz
 ```
 Then to run it, execute the following in the terminal:
 ```
 wudz-lit
 ```
 
 ### Usage
```

### Comparing `wuddz_lit-1.0.0/pyproject.toml` & `wuddz_lit-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 only-include = ["wuddz_lit"]
 
 [project]
 name = "wuddz_lit"
-version = "1.0.0"
+version = "1.0.1"
 description = "Wuddz-Lit Is An Awesome & Quite Efficient Literotica.com Author/Category/Audio/Illustration Stories Downloader."
 readme = "README.md"
 authors = [
   { name="Wuddz-Devs", email="wuddz_devs@protonmail.com" },
 ]
 
 license = { file = "LICENSE" }
```

### Comparing `wuddz_lit-1.0.0/PKG-INFO` & `wuddz_lit-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wuddz_lit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wuddz-Lit Is An Awesome & Quite Efficient Literotica.com Author/Category/Audio/Illustration Stories Downloader.
 Project-URL: Homepage, https://github.com/wuddz-devs/wuddz-lit
 Author-email: Wuddz-Devs <wuddz_devs@protonmail.com>
 License: MIT License
         
         Copyright (c) 2024 Wuddz-Devs
         
@@ -47,15 +47,15 @@
 ## Installation
 Install using [PyPI](https://pypi.org/project/wuddz-lit):
 ```
 pip install wuddz-lit
 ```
 Install locally by cloning or downloading and extracting the repo, then cd into 'dist' directory and execute:
 ```
-pip install wuddz_lit-1.0.0.tar.gz
+pip install wuddz_lit-1.0.1.tar.gz
 ```
 Then to run it, execute the following in the terminal:
 ```
 wudz-lit
 ```
 
 ### Usage
```

