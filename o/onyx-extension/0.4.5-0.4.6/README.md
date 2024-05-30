# Comparing `tmp/onyx_extension-0.4.5.tar.gz` & `tmp/onyx_extension-0.4.6.tar.gz`

## Comparing `onyx_extension-0.4.5.tar` & `onyx_extension-0.4.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/.yarnrc.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/Untitled.ipynb
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/Untitled1.ipynb
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/build.bat
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/install.json
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/tsconfig.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/jupyter-config/server-config/onyx_extension.json
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/_version.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/handlers.py
--rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/build_log.json
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/package.json
--rw-r--r--   0        0        0    16130 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js.map
--rw-r--r--   0        0        0    30675 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/remoteEntry.d7e1768430c684ce7518.js
--rw-r--r--   0        0        0    29403 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/remoteEntry.d7e1768430c684ce7518.js.map
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/style.js
--rw-r--r--   0        0        0    35304 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map
--rw-r--r--   0        0        0  1084836 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js
--rw-r--r--   0        0        0    82077 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map
--rw-r--r--   0        0        0   570227 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js
--rw-r--r--   0        0        0   670422 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/src/App.tsx
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/src/handler.ts
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/src/icon.ts
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/src/index.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/src/typings.d.ts
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/src/widget.tsx
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/style/base.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/style/index.css
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/style/index.js
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/style/icons/dna.svg
--rw-r--r--   0        0        0   207294 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/tmp/C-B01922D432_scylla_report.html
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/README.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 onyx_extension-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/.yarnrc.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/Untitled.ipynb
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/Untitled1.ipynb
+-rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/build.bat
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/install.json
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/tsconfig.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/jupyter-config/server-config/onyx_extension.json
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/_version.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/handlers.py
+-rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/build_log.json
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/package.json
+-rw-r--r--   0        0        0    16130 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js.map
+-rw-r--r--   0        0        0    30675 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/remoteEntry.1c17a04832b25d4fbc2e.js
+-rw-r--r--   0        0        0    29403 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/remoteEntry.1c17a04832b25d4fbc2e.js.map
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/style.js
+-rw-r--r--   0        0        0    35304 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map
+-rw-r--r--   0        0        0  1084836 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js
+-rw-r--r--   0        0        0    82077 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map
+-rw-r--r--   0        0        0   570227 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js
+-rw-r--r--   0        0        0   670422 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/src/App.tsx
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/src/handler.ts
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/src/icon.ts
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/src/index.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/src/typings.d.ts
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/src/widget.tsx
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/style/base.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/style/index.css
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/style/index.js
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/style/icons/dna.svg
+-rw-r--r--   0        0        0   207294 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/tmp/C-B01922D432_scylla_report.html
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/README.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 onyx_extension-0.4.6/PKG-INFO
```

### Comparing `onyx_extension-0.4.5/Untitled1.ipynb` & `onyx_extension-0.4.6/Untitled1.ipynb`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/package.json` & `onyx_extension-0.4.6/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.6'"}*

```diff
@@ -197,9 +197,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.5"
+    "version": "0.4.6"
 }
```

### Comparing `onyx_extension-0.4.5/tsconfig.json` & `onyx_extension-0.4.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/__init__.py` & `onyx_extension-0.4.6/onyx_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/handlers.py` & `onyx_extension-0.4.6/onyx_extension/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     # The following decorator should be present on all verb methods (head, get, post,
     # patch, put, delete, options) to ensure only authorized user can request the
     # Jupyter server
     @tornado.web.authenticated
     def get(self):
         try:
             
-            s3location = self.get_query_argument("s3location")
-            temp_file = self._copy_s3_file(s3location)
+            s3location = 'a'
+            temp_file = 'b'
             self.finish(json.dumps({
                 "location": s3location,
                 "temp_file": temp_file
             }))
         except Exception as e:
             self.finish(json.dumps({
                 "exception": e
```

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/build_log.json` & `onyx_extension-0.4.6/onyx_extension/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993827160494%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'onyx_extension': {'version': '0.4.6'}}}}}}"}*

```diff
@@ -661,15 +661,15 @@
                             "requiredVersion": "^2.49.2",
                             "singleton": true
                         },
                         "climb-onyx-ui": {},
                         "onyx_extension": {
                             "import": "C:\\Users\\butchena\\Documents\\projects\\CLIMB-TRE(FCOD-LOMAN-NJ-1)\\gitlab\\onyx-extension\\lib\\index.js",
                             "singleton": true,
-                            "version": "0.4.5"
+                            "version": "0.4.6"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/package.json` & `onyx_extension-0.4.6/onyx_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static\\\\remoteEntry.1c17a04832b25d4fbc2e.js'}}",*

 * * "'version'": "'0.4.6'"}*

```diff
@@ -106,15 +106,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/extension-onyx_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static\\remoteEntry.d7e1768430c684ce7518.js",
+            "load": "static\\remoteEntry.1c17a04832b25d4fbc2e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "onyx_extension"
                 },
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.5"
+    "version": "0.4.6"
 }
```

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js` & `onyx_extension-0.4.6/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js.map` & `onyx_extension-0.4.6/onyx_extension/labextension/static/lib_index_js.c9b19544a878d8e8f881.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/remoteEntry.d7e1768430c684ce7518.js` & `onyx_extension-0.4.6/onyx_extension/labextension/static/remoteEntry.1c17a04832b25d4fbc2e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -432,15 +432,15 @@
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
                     register("climb-onyx-ui", "0.4.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js */ "./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js"))))));
                     /******/
-                    register("onyx_extension", "0.4.5", () => (Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("onyx_extension", "0.4.6", () => (Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1118,8 +1118,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/onyx_extension");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).onyx_extension = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.d7e1768430c684ce7518.js.map
+//# sourceMappingURL=remoteEntry.1c17a04832b25d4fbc2e.js.map
```

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/remoteEntry.d7e1768430c684ce7518.js.map` & `onyx_extension-0.4.6/onyx_extension/labextension/static/remoteEntry.1c17a04832b25d4fbc2e.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.1c17a04832b25d4fbc2e.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.d7e1768430c684ce7518.js",
+    "file": "remoteEntry.1c17a04832b25d4fbc2e.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,mbAAmb;WACjd;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WC9LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://onyx_extension/webpack/container-entry",
         "webpack://onyx_extension/webpack/bootstrap",
         "webpack://onyx_extension/webpack/runtime/compat get default export",
@@ -30,15 +30,15 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"webpack_sharing_consume_default_react\":\"b6171cc67744114369b8\",\"lib_index_js\":\"c9b19544a878d8e8f881\",\"vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d\":\"daff3ca64e09afb815f2\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9\":\"e7e279648ddef5dfd55a\",\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\":\"32d25ee4ef05954a5218\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"onyx_extension:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"onyx_extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"climb-onyx-ui\", \"0.4.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js */ \"./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js\"))))));\n\t\t\tregister(\"onyx_extension\", \"0.4.5\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"onyx_extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"climb-onyx-ui\", \"0.4.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js */ \"./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js\"))))));\n\t\t\tregister(\"onyx_extension\", \"0.4.6\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/docmanager\", [1,4,1,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,1,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,1,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,1,8])),\n\t\"webpack/sharing/consume/default/climb-onyx-ui/climb-onyx-ui\": () => (loadStrictVersionCheckFallback(\"default\", \"climb-onyx-ui\", [2,0,4,0], () => (__webpack_require__.e(\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\").then(() => (() => (__webpack_require__(/*! climb-onyx-ui */ \"./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,8]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/climb-onyx-ui/climb-onyx-ui\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
         "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"onyx_extension\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(\"webpack_sharing_consume_default_react\" != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkonyx_extension\"] = self[\"webpackChunkonyx_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/onyx_extension\");\n",
         ""
```

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js` & `onyx_extension-0.4.6/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map` & `onyx_extension-0.4.6/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js` & `onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map` & `onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js` & `onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map` & `onyx_extension-0.4.6/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/src/handler.ts` & `onyx_extension-0.4.6/src/handler.ts`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/src/index.ts` & `onyx_extension-0.4.6/src/index.ts`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/style/icons/dna.svg` & `onyx_extension-0.4.6/style/icons/dna.svg`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/tmp/C-B01922D432_scylla_report.html` & `onyx_extension-0.4.6/tmp/C-B01922D432_scylla_report.html`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/.gitignore` & `onyx_extension-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/pyproject.toml` & `onyx_extension-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.5/PKG-INFO` & `onyx_extension-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: onyx_extension
-Version: 0.4.5
+Version: 0.4.6
 Dynamic: Keywords
 Summary: A minimal JupyterLab extension with backend and frontend parts.
 Project-URL: Homepage, https://github.com/jupyterlab/extension-onyx_extension
 Project-URL: Bug Tracker, https://github.com/jupyterlab/extension-onyx_extension/issues
 Project-URL: Repository, https://github.com/jupyterlab/extension-onyx_extension.git
 Author: Project Jupyter Contributors
 License: MIT
```

