# Comparing `tmp/jpfiddle_extension-0.1.0.tar.gz` & `tmp/jpfiddle_extension-0.1.4.tar.gz`

## Comparing `jpfiddle_extension-0.1.0.tar` & `jpfiddle_extension-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/install.json
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/tsconfig.json
--rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/yarn.lock
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/_version.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/509.b7c67fe38bb208768f2a.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/remoteEntry.b46f4a0e01f00fc3172f.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/style/index.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/LICENSE
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/README.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.copier-answers.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/RELEASE.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/install.json
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/tsconfig.json
+-rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/yarn.lock
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/_version.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/package.json
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/509.a4695b98757ae7ffb15f.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/remoteEntry.80be61ad8cf097caafa4.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/style/index.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.4/PKG-INFO
```

### Comparing `jpfiddle_extension-0.1.0/RELEASE.md` & `jpfiddle_extension-0.1.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/package.json` & `jpfiddle_extension-0.1.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.4'"}*

```diff
@@ -179,9 +179,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.4"
 }
```

### Comparing `jpfiddle_extension-0.1.0/tsconfig.json` & `jpfiddle_extension-0.1.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/yarn.lock` & `jpfiddle_extension-0.1.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/jpfiddle_extension/__init__.py` & `jpfiddle_extension-0.1.4/jpfiddle_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/package.json` & `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.80be61ad8cf097caafa4.js'}}",*

 * * "'version'": "'0.1.4'"}*

```diff
@@ -99,15 +99,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/magland/jpfiddle_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b46f4a0e01f00fc3172f.js",
+            "load": "static/remoteEntry.80be61ad8cf097caafa4.js",
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
-    "version": "0.1.0"
+    "version": "0.1.4"
 }
```

### Comparing `jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js` & `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/remoteEntry.b46f4a0e01f00fc3172f.js` & `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/remoteEntry.80be61ad8cf097caafa4.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -43,49 +43,49 @@
         }), r
     }, o.d = (e, r) => {
         for (var t in r) o.o(r, t) && !o.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, o.f = {}, o.e = e => Promise.all(Object.keys(o.f).reduce(((r, t) => (o.f[t](e, r), r)), [])), o.u = e => e + "." + {
-        509: "b7c67fe38bb208768f2a",
+        509: "a4695b98757ae7ffb15f",
         728: "151b68248be6f9ed2608"
     } [e] + ".js?v=" + {
-        509: "b7c67fe38bb208768f2a",
+        509: "a4695b98757ae7ffb15f",
         728: "151b68248be6f9ed2608"
     } [e], o.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), o.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jpfiddle_extension:", o.l = (t, n, i, a) => {
         if (e[t]) e[t].push(n);
         else {
             var d, l;
             if (void 0 !== i)
-                for (var s = document.getElementsByTagName("script"), c = 0; c < s.length; c++) {
-                    var f = s[c];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + i) {
-                        d = f;
+                for (var s = document.getElementsByTagName("script"), u = 0; u < s.length; u++) {
+                    var c = s[u];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + i) {
+                        d = c;
                         break
                     }
                 }
             d || (l = !0, (d = document.createElement("script")).charset = "utf-8", d.timeout = 120, o.nc && d.setAttribute("nonce", o.nc), d.setAttribute("data-webpack", r + i), d.src = t), e[t] = [n];
-            var u = (r, n) => {
+            var f = (r, n) => {
                     d.onerror = d.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], d.parentNode && d.parentNode.removeChild(d), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(u.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: d
                 }), 12e4);
-            d.onerror = u.bind(null, d.onerror), d.onload = u.bind(null, d.onload), l && document.head.appendChild(d)
+            d.onerror = f.bind(null, d.onerror), d.onload = f.bind(null, d.onload), l && document.head.appendChild(d)
         }
     }, o.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var i = a[e] = a[e] || {},
                         l = i[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : d > l.from)) && (i[r] = {
                         get: () => o.e(509).then((() => () => o(509))),
                         from: d,
                         eager: !1
                     })
-                })("jpfiddle_extension", "0.1.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jpfiddle_extension", "0.1.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         o.g.importScripts && (e = o.g.location + "");
         var r = o.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jpfiddle_extension-0.1.0/jpfiddle_extension/labextension/static/third-party-licenses.json` & `jpfiddle_extension-0.1.4/jpfiddle_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/.gitignore` & `jpfiddle_extension-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/LICENSE` & `jpfiddle_extension-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/README.md` & `jpfiddle_extension-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/pyproject.toml` & `jpfiddle_extension-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.0/PKG-INFO` & `jpfiddle_extension-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jpfiddle_extension
-Version: 0.1.0
+Version: 0.1.4
 Dynamic: Keywords
 Summary: A JupyterLab extension for jpfiddle.
 Project-URL: Homepage, https://github.com/magland/jpfiddle_extension
 Project-URL: Bug Tracker, https://github.com/magland/jpfiddle_extension/issues
 Project-URL: Repository, https://github.com/magland/jpfiddle_extension.git
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License: BSD 3-Clause License
```

