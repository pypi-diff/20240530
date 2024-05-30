# Comparing `tmp/jpfiddle_extension-0.1.5.tar.gz` & `tmp/jpfiddle_extension-0.1.6.tar.gz`

## Comparing `jpfiddle_extension-0.1.5.tar` & `jpfiddle_extension-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.copier-answers.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/install.json
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/tsconfig.json
--rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/yarn.lock
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/_version.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/package.json
--rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/509.24f9b6cff68605990ed0.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/remoteEntry.8b8e18d0102323e7a700.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/style/index.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/LICENSE
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/README.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/.copier-answers.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/RELEASE.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/install.json
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/tsconfig.json
+-rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/yarn.lock
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/_version.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/package.json
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/509.c92db09e63441ab720ab.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/remoteEntry.4a65306b511397db6774.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/style/index.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.6/PKG-INFO
```

### Comparing `jpfiddle_extension-0.1.5/RELEASE.md` & `jpfiddle_extension-0.1.6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/package.json` & `jpfiddle_extension-0.1.6/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.6'"}*

```diff
@@ -179,9 +179,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `jpfiddle_extension-0.1.5/tsconfig.json` & `jpfiddle_extension-0.1.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/yarn.lock` & `jpfiddle_extension-0.1.6/yarn.lock`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/jpfiddle_extension/__init__.py` & `jpfiddle_extension-0.1.6/jpfiddle_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/package.json` & `jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.4a65306b511397db6774.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -99,15 +99,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/magland/jpfiddle_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8b8e18d0102323e7a700.js",
+            "load": "static/remoteEntry.4a65306b511397db6774.js",
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
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/509.24f9b6cff68605990ed0.js` & `jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/509.c92db09e63441ab720ab.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -75,15 +75,18 @@
                                     if ("" !== t) try {
                                         await e.serviceManager.contents.get(t)
                                     } catch (e) {
                                         return void window.parent.postMessage({
                                             type: "files",
                                             files: null
                                         }, "*")
-                                    }
+                                    } else if (0 === (await e.serviceManager.contents.get("")).content.length) return void window.parent.postMessage({
+                                        type: "files",
+                                        files: null
+                                    }, "*");
                                     console.log("Getting files in directory:", t);
                                     const n = async t => {
                                         const o = [],
                                             a = await e.serviceManager.contents.get(t);
                                         if (a)
                                             for (const t of a.content)
                                                 if ("directory" === t.type) o.push(...await n(t.path));
```

### Comparing `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js` & `jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/remoteEntry.8b8e18d0102323e7a700.js` & `jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/remoteEntry.4a65306b511397db6774.js`

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
-        509: "24f9b6cff68605990ed0",
+        509: "c92db09e63441ab720ab",
         728: "151b68248be6f9ed2608"
     } [e] + ".js?v=" + {
-        509: "24f9b6cff68605990ed0",
+        509: "c92db09e63441ab720ab",
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
-                })("jpfiddle_extension", "0.1.5"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jpfiddle_extension", "0.1.6"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         o.g.importScripts && (e = o.g.location + "");
         var r = o.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jpfiddle_extension-0.1.5/jpfiddle_extension/labextension/static/third-party-licenses.json` & `jpfiddle_extension-0.1.6/jpfiddle_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/src/index.ts` & `jpfiddle_extension-0.1.6/src/index.ts`

 * *Files 4% similar despite different names*

```diff
@@ -194,22 +194,31 @@
   };
 
   const postFilesToParent = async () => {
     if (fiddleId === undefined) {
       console.error('No fiddleId found in get-files event');
       return;
     }
+
     // check whether directory exists
+    // if it doesn't, send null to signal that we should receive files
     if (fiddleId !== '') {
       try {
         await app.serviceManager.contents.get(fiddleId);
       } catch (error) {
         window.parent.postMessage({ type: 'files', files: null }, '*');
         return;
       }
+    } else {
+      // check whether the directory is empty
+      const a = await app.serviceManager.contents.get('');
+      if (a.content.length === 0) {
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
```

### Comparing `jpfiddle_extension-0.1.5/.gitignore` & `jpfiddle_extension-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/LICENSE` & `jpfiddle_extension-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/README.md` & `jpfiddle_extension-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/pyproject.toml` & `jpfiddle_extension-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.5/PKG-INFO` & `jpfiddle_extension-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jpfiddle_extension
-Version: 0.1.5
+Version: 0.1.6
 Dynamic: Keywords
 Summary: A JupyterLab extension for jpfiddle.
 Project-URL: Homepage, https://github.com/magland/jpfiddle_extension
 Project-URL: Bug Tracker, https://github.com/magland/jpfiddle_extension/issues
 Project-URL: Repository, https://github.com/magland/jpfiddle_extension.git
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License: BSD 3-Clause License
```

