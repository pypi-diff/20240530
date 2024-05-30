# Comparing `tmp/jpfiddle_extension-0.1.4.tar.gz` & `tmp/jpfiddle_extension-0.1.5.tar.gz`

## Comparing `jpfiddle_extension-0.1.4.tar` & `jpfiddle_extension-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.copier-answers.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/install.json
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/tsconfig.json
--rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/yarn.lock
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/_version.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/package.json
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/509.a4695b98757ae7ffb15f.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/remoteEntry.80be61ad8cf097caafa4.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/style/index.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/LICENSE
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/README.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.copier-answers.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/RELEASE.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/install.json
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/tsconfig.json
+-rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/yarn.lock
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/_version.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/package.json
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/509.24f9b6cff68605990ed0.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/remoteEntry.8b8e18d0102323e7a700.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/style/index.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/PKG-INFO
```

### Comparing `jpfiddle_extension-0.1.4/RELEASE.md` & `jpfiddle_extension-0.1.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/package.json` & `jpfiddle_extension-0.1.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.5'"}*

```diff
@@ -179,9 +179,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `jpfiddle_extension-0.1.4/tsconfig.json` & `jpfiddle_extension-0.1.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/yarn.lock` & `jpfiddle_extension-0.1.5/yarn.lock`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/jpfiddle_extension/__init__.py` & `jpfiddle_extension-0.1.5/jpfiddle_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/package.json` & `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.8b8e18d0102323e7a700.js'}}",*

 * * "'version'": "'0.1.5'"}*

```diff
@@ -99,15 +99,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/magland/jpfiddle_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.80be61ad8cf097caafa4.js",
+            "load": "static/remoteEntry.8b8e18d0102323e7a700.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jpfiddle_extension/labextension"
     },
     "keywords": [
         "jupyter",
@@ -184,9 +184,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/509.a4695b98757ae7ffb15f.js` & `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/509.24f9b6cff68605990ed0.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -11,71 +11,72 @@
                     autoStart: !0,
                     activate: e => {
                         console.log("ACTIVATING: JupyterLab extension jpfiddle_extension is activating."),
                             function(e) {
                                 if (!window.parent) return void console.error("No parent window found for jpfiddle-extension");
                                 let t;
                                 e.serviceManager.contents.fileChanged.connect((async (n, o) => {
-                                    if (console.info("File changed:", o), t)
+                                    if (console.info("File changed:", o), void 0 !== t)
                                         if ("save" === o.type && o.newValue) {
                                             if ("directory" === o.newValue.type) return;
                                             const n = o.newValue.path;
                                             if (!n) return void console.warn("No file path found in fileChanged event");
-                                            if (!n.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", n, t);
-                                            const i = n.slice(t.length + 1);
+                                            if ("" !== t && !n.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", n, t);
+                                            const i = "" !== t ? n.slice(t.length + 1) : n;
                                             console.log("File saved:", i, o);
                                             const a = await e.serviceManager.contents.get(n);
                                             window.parent.postMessage({
                                                 type: "file-saved",
                                                 path: i,
                                                 content: a.content
                                             }, "*")
                                         } else if ("delete" === o.type && o.oldValue) {
                                         const e = o.oldValue.path;
                                         if (!e) return void console.warn("No file path found in fileChanged event");
-                                        if (!e.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, t);
-                                        const n = e.slice(t.length + 1);
+                                        if ("" !== t && !e.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, t);
+                                        const n = "" !== t ? e.slice(t.length + 1) : e;
                                         console.log("File deleted:", n, o), window.parent.postMessage({
                                             type: "file-deleted",
                                             path: n
                                         }, "*")
                                     } else if ("rename" === o.type && o.oldValue && o.newValue) {
                                         const e = o.oldValue.path,
                                             n = o.newValue.path;
                                         if (!e || !n) return void console.warn("No file path found in fileChanged event");
-                                        if (!e.startsWith(t + "/") || !n.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, n, t);
-                                        const i = e.slice(t.length + 1),
-                                            a = n.slice(t.length + 1);
+                                        if ("" !== t && !e.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, t);
+                                        if ("" !== t && !n.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", n, t);
+                                        const i = "" !== t ? e.slice(t.length + 1) : e,
+                                            a = "" !== t ? n.slice(t.length + 1) : n;
                                         console.log("File renamed:", i, a, o), window.parent.postMessage({
                                             type: "file-renamed",
                                             oldPath: i,
                                             newPath: a
                                         }, "*")
                                     } else if ("new" === o.type && o.newValue) {
                                         const e = o.newValue.path;
                                         if (!e) return void console.warn("No file path found in fileChanged event");
-                                        if (!e.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, t);
-                                        const n = e.slice(t.length + 1);
+                                        if ("" !== t && !e.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, t);
+                                        const n = "" !== t ? e.slice(t.length + 1) : e;
                                         window.parent.postMessage({
                                             type: "file-created",
                                             path: n
                                         }, "*")
                                     } else console.warn(`Unknown change type: ${o.type}`);
                                     else console.error("No fiddleId found in fileChanged event")
                                 }));
                                 const n = async () => {
-                                    if (t) {
+                                    if (void 0 !== t) {
                                         for (let t = 0; t < 100 && (await new Promise((e => setTimeout(e, 100))), !e.commands.hasCommand("filebrowser:go-to-path")); t++);
                                         e.commands.hasCommand("filebrowser:go-to-path") ? await e.commands.execute("filebrowser:go-to-path", {
                                             path: t
                                         }) : console.error("Command filebrowser:go-to-path not found")
                                     } else console.error("No fiddleId found in changeToFiddleDirectory")
                                 }, o = async () => {
-                                    if (!t) return void console.error("No fiddleId found in get-files event");
-                                    try {
+                                    if (void 0 === t) return void console.error("No fiddleId found in get-files event");
+                                    if ("" !== t) try {
                                         await e.serviceManager.contents.get(t)
                                     } catch (e) {
                                         return void window.parent.postMessage({
                                             type: "files",
                                             files: null
                                         }, "*")
                                     }
@@ -96,40 +97,40 @@
                                                         path: t.path,
                                                         content: n
                                                     })
                                                 } return o
                                     }, o = await n(t);
                                     console.log("Sending files:", o);
                                     const a = o.map((e => ({
-                                        path: e.path.slice((t || "").length + 1),
+                                        path: "" !== t ? e.path.slice((t || "").length + 1) : e.path,
                                         content: e.content
                                     })));
                                     window.parent.postMessage({
                                         type: "files",
                                         files: a
                                     }, "*")
                                 };
                                 window.addEventListener("message", (async i => {
                                     const l = i.data;
                                     if (console.log("Message received in the iframe:", l), "set-fiddle-id" === l.type) {
-                                        if (t = l.fiddleId, !t) return;
+                                        if (t = l.fiddleId, void 0 === t) return;
                                         n()
                                     } else if ("set-files" === l.type) {
-                                        if (!t) return void console.error("No fiddleId found in set-files event");
-                                        try {
+                                        if (void 0 === t) return void console.error("No fiddleId found in set-files event");
+                                        if ("" !== t) try {
                                             await e.serviceManager.contents.get(t)
                                         } catch (n) {
                                             console.log("Creating directory:", t), await e.serviceManager.contents.save(t, {
                                                 type: "directory",
                                                 name: a(t)
                                             })
                                         }
                                         const l = i.data.files;
                                         for (const n of l) {
-                                            const o = t + "/" + n.path;
+                                            const o = "" !== t ? t + "/" + n.path : n.path;
                                             if (o.split("/").length > 1 && await s(e, o.split("/").slice(0, -1).join("/")), null !== n.content) console.log("saving file", o), await e.serviceManager.contents.save(o, {
                                                 type: "file",
                                                 format: "text",
                                                 name: a(o),
                                                 content: n.content
                                             });
                                             else try {
```

### Comparing `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js` & `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/remoteEntry.80be61ad8cf097caafa4.js` & `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/remoteEntry.8b8e18d0102323e7a700.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, o.d = (e, r) => {
         for (var t in r) o.o(r, t) && !o.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, o.f = {}, o.e = e => Promise.all(Object.keys(o.f).reduce(((r, t) => (o.f[t](e, r), r)), [])), o.u = e => e + "." + {
-        509: "a4695b98757ae7ffb15f",
+        509: "24f9b6cff68605990ed0",
         728: "151b68248be6f9ed2608"
     } [e] + ".js?v=" + {
-        509: "a4695b98757ae7ffb15f",
+        509: "24f9b6cff68605990ed0",
         728: "151b68248be6f9ed2608"
     } [e], o.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var i = a[e] = a[e] || {},
                         l = i[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : d > l.from)) && (i[r] = {
                         get: () => o.e(509).then((() => () => o(509))),
                         from: d,
                         eager: !1
                     })
-                })("jpfiddle_extension", "0.1.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jpfiddle_extension", "0.1.5"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         o.g.importScripts && (e = o.g.location + "");
         var r = o.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/third-party-licenses.json` & `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/src/index.ts` & `jpfiddle_extension-0.1.5/src/index.ts`

 * *Files 13% similar despite different names*

```diff
@@ -30,37 +30,38 @@
     return;
   }
   let fiddleId: string | undefined = undefined;
 
   // handle file changes
   app.serviceManager.contents.fileChanged.connect(async (sender, change) => {
     console.info('File changed:', change);
-    if (!fiddleId) {
+    if (fiddleId === undefined) {
       console.error('No fiddleId found in fileChanged event');
       return;
     }
     if (change.type === 'save' && change.newValue) {
       // ignore if it's a directory
       if (change.newValue.type === 'directory') {
         return;
       }
       const fullPath = change.newValue.path;
       if (!fullPath) {
         console.warn('No file path found in fileChanged event');
         return;
       }
-      if (!fullPath.startsWith(fiddleId + '/')) {
+      if (fiddleId !== '' && !fullPath.startsWith(fiddleId + '/')) {
         console.warn(
           'File path does not start with fiddleId:',
           fullPath,
           fiddleId
         );
         return;
       }
-      const path = fullPath.slice(fiddleId.length + 1);
+      const path =
+        fiddleId !== '' ? fullPath.slice(fiddleId.length + 1) : fullPath;
       console.log('File saved:', path, change);
       const vv = await app.serviceManager.contents.get(fullPath);
       window.parent.postMessage(
         {
           type: 'file-saved',
           path,
           content: vv.content
@@ -69,23 +70,24 @@
       );
     } else if (change.type === 'delete' && change.oldValue) {
       const fullPath = change.oldValue.path;
       if (!fullPath) {
         console.warn('No file path found in fileChanged event');
         return;
       }
-      if (!fullPath.startsWith(fiddleId + '/')) {
+      if (fiddleId !== '' && !fullPath.startsWith(fiddleId + '/')) {
         console.warn(
           'File path does not start with fiddleId:',
           fullPath,
           fiddleId
         );
         return;
       }
-      const path = fullPath.slice(fiddleId.length + 1);
+      const path =
+        fiddleId !== '' ? fullPath.slice(fiddleId.length + 1) : fullPath;
       console.log('File deleted:', path, change);
       window.parent.postMessage(
         {
           type: 'file-deleted',
           path
         },
         '*'
@@ -93,28 +95,34 @@
     } else if (change.type === 'rename' && change.oldValue && change.newValue) {
       const oldFullPath = change.oldValue.path;
       const newFullPath = change.newValue.path;
       if (!oldFullPath || !newFullPath) {
         console.warn('No file path found in fileChanged event');
         return;
       }
-      if (
-        !oldFullPath.startsWith(fiddleId + '/') ||
-        !newFullPath.startsWith(fiddleId + '/')
-      ) {
+      if (fiddleId !== '' && !oldFullPath.startsWith(fiddleId + '/')) {
         console.warn(
           'File path does not start with fiddleId:',
           oldFullPath,
+          fiddleId
+        );
+        return;
+      }
+      if (fiddleId !== '' && !newFullPath.startsWith(fiddleId + '/')) {
+        console.warn(
+          'File path does not start with fiddleId:',
           newFullPath,
           fiddleId
         );
         return;
       }
-      const oldPath = oldFullPath.slice(fiddleId.length + 1);
-      const newPath = newFullPath.slice(fiddleId.length + 1);
+      const oldPath =
+        fiddleId !== '' ? oldFullPath.slice(fiddleId.length + 1) : oldFullPath;
+      const newPath =
+        fiddleId !== '' ? newFullPath.slice(fiddleId.length + 1) : newFullPath;
       console.log('File renamed:', oldPath, newPath, change);
       window.parent.postMessage(
         {
           type: 'file-renamed',
           oldPath,
           newPath
         },
@@ -122,38 +130,39 @@
       );
     } else if (change.type === 'new' && change.newValue) {
       const fullPath = change.newValue.path;
       if (!fullPath) {
         console.warn('No file path found in fileChanged event');
         return;
       }
-      if (!fullPath.startsWith(fiddleId + '/')) {
+      if (fiddleId !== '' && !fullPath.startsWith(fiddleId + '/')) {
         console.warn(
           'File path does not start with fiddleId:',
           fullPath,
           fiddleId
         );
         return;
       }
-      const path = fullPath.slice(fiddleId.length + 1);
+      const path =
+        fiddleId !== '' ? fullPath.slice(fiddleId.length + 1) : fullPath;
       window.parent.postMessage(
         {
           type: 'file-created',
           path
         },
         '*'
       );
     } else {
       console.warn(`Unknown change type: ${change.type}`);
     }
   });
 
   // helper functions
   const changeToFiddleDirectory = async () => {
-    if (!fiddleId) {
+    if (fiddleId === undefined) {
       console.error('No fiddleId found in changeToFiddleDirectory');
       return;
     }
     // the command to go-to-path is not available immediately
     // we need to wait until the file browser is ready
     // so we will retry every 0.1 seconds for 10 seconds
     for (let i = 0; i < 100; i++) {
@@ -181,24 +190,26 @@
       console.error('Command application:close-all not found');
       return;
     }
     await app.commands.execute('application:close-all');
   };
 
   const postFilesToParent = async () => {
-    if (!fiddleId) {
+    if (fiddleId === undefined) {
       console.error('No fiddleId found in get-files event');
       return;
     }
     // check whether directory exists
-    try {
-      await app.serviceManager.contents.get(fiddleId);
-    } catch (error) {
-      window.parent.postMessage({ type: 'files', files: null }, '*');
-      return;
+    if (fiddleId !== '') {
+      try {
+        await app.serviceManager.contents.get(fiddleId);
+      } catch (error) {
+        window.parent.postMessage({ type: 'files', files: null }, '*');
+        return;
+      }
     }
     console.log('Getting files in directory:', fiddleId);
     const getFilesInDirectory = async (
       path: string
     ): Promise<{ path: string; content: string }[]> => {
       const files: { path: string; content: string }[] = [];
       const a = await app.serviceManager.contents.get(path);
@@ -219,49 +230,52 @@
       }
       return files;
     };
     const files: { path: string; content: string }[] =
       await getFilesInDirectory(fiddleId);
     console.log('Sending files:', files);
     const files2 = files.map(f => ({
-      path: f.path.slice((fiddleId || '').length + 1),
+      path:
+        fiddleId !== '' ? f.path.slice((fiddleId || '').length + 1) : f.path,
       content: f.content
     }));
     window.parent.postMessage({ type: 'files', files: files2 }, '*');
   };
 
   /* Incoming messages management */
   window.addEventListener('message', async event => {
     const msg = event.data;
     console.log('Message received in the iframe:', msg);
     if (msg.type === 'set-fiddle-id') {
       fiddleId = msg.fiddleId;
-      if (!fiddleId) {
+      if (fiddleId === undefined) {
         return;
       }
 
       changeToFiddleDirectory();
     } else if (msg.type === 'set-files') {
-      if (!fiddleId) {
+      if (fiddleId === undefined) {
         console.error('No fiddleId found in set-files event');
         return;
       }
       // create the fiddle directory if it doesn't exist
-      try {
-        await app.serviceManager.contents.get(fiddleId);
-      } catch (error) {
-        console.log('Creating directory:', fiddleId);
-        await app.serviceManager.contents.save(fiddleId, {
-          type: 'directory',
-          name: baseName(fiddleId)
-        });
+      if (fiddleId !== '') {
+        try {
+          await app.serviceManager.contents.get(fiddleId);
+        } catch (error) {
+          console.log('Creating directory:', fiddleId);
+          await app.serviceManager.contents.save(fiddleId, {
+            type: 'directory',
+            name: baseName(fiddleId)
+          });
+        }
       }
       const files = event.data.files;
       for (const file of files) {
-        const path = fiddleId + '/' + file.path;
+        const path = fiddleId !== '' ? fiddleId + '/' + file.path : file.path;
         if (path.split('/').length > 1) {
           await ensureDirectoryExists(
             app,
             path.split('/').slice(0, -1).join('/')
           );
         }
         if (file.content !== null) {
```

### Comparing `jpfiddle_extension-0.1.4/.gitignore` & `jpfiddle_extension-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/LICENSE` & `jpfiddle_extension-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/README.md` & `jpfiddle_extension-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/pyproject.toml` & `jpfiddle_extension-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.4/PKG-INFO` & `jpfiddle_extension-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jpfiddle_extension
-Version: 0.1.4
+Version: 0.1.5
 Dynamic: Keywords
 Summary: A JupyterLab extension for jpfiddle.
 Project-URL: Homepage, https://github.com/magland/jpfiddle_extension
 Project-URL: Bug Tracker, https://github.com/magland/jpfiddle_extension/issues
 Project-URL: Repository, https://github.com/magland/jpfiddle_extension.git
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License: BSD 3-Clause License
```

