# Comparing `tmp/onyx_extension-0.4.1.tar.gz` & `tmp/onyx_extension-0.4.2.tar.gz`

## Comparing `onyx_extension-0.4.1.tar` & `onyx_extension-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/.yarnrc.yml
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/build.bat
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/install.json
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/tsconfig.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/jupyter-config/server-config/onyx_extension.json
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/_version.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/handlers.py
--rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/build_log.json
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/package.json
--rw-r--r--   0        0        0    15547 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/lib_index_js.4bae6e3d1c04b0e96d5c.js
--rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/lib_index_js.4bae6e3d1c04b0e96d5c.js.map
--rw-r--r--   0        0        0    30454 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/remoteEntry.0fa3b8b49d2409fd11bb.js
--rw-r--r--   0        0        0    29181 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/remoteEntry.0fa3b8b49d2409fd11bb.js.map
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/style.js
--rw-r--r--   0        0        0    35304 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map
--rw-r--r--   0        0        0  1084836 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js
--rw-r--r--   0        0        0    82077 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map
--rw-r--r--   0        0        0   570227 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js
--rw-r--r--   0        0        0   670422 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/src/App.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/src/handler.ts
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/src/icon.ts
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/src/index.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/src/typings.d.ts
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/src/widget.tsx
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/style/base.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/style/index.css
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/style/index.js
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/style/icons/dna.svg
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/README.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 onyx_extension-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/.yarnrc.yml
+-rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/build.bat
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/install.json
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/tsconfig.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/jupyter-config/server-config/onyx_extension.json
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/_version.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/handlers.py
+-rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/build_log.json
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/package.json
+-rw-r--r--   0        0        0    15674 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/lib_index_js.387211c2f04c65e8ccd7.js
+-rw-r--r--   0        0        0    10034 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/lib_index_js.387211c2f04c65e8ccd7.js.map
+-rw-r--r--   0        0        0    30454 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/remoteEntry.8132ef2cf277548ef51c.js
+-rw-r--r--   0        0        0    29181 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/remoteEntry.8132ef2cf277548ef51c.js.map
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/style.js
+-rw-r--r--   0        0        0    35304 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map
+-rw-r--r--   0        0        0  1084836 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js
+-rw-r--r--   0        0        0    82077 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map
+-rw-r--r--   0        0        0   570227 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js
+-rw-r--r--   0        0        0   670422 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/src/App.tsx
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/src/handler.ts
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/src/icon.ts
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/src/index.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/src/typings.d.ts
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/src/widget.tsx
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/style/base.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/style/index.css
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/style/index.js
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/style/icons/dna.svg
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/README.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 onyx_extension-0.4.2/PKG-INFO
```

### Comparing `onyx_extension-0.4.1/package.json` & `onyx_extension-0.4.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.4.2'"}*

```diff
@@ -197,9 +197,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `onyx_extension-0.4.1/tsconfig.json` & `onyx_extension-0.4.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/__init__.py` & `onyx_extension-0.4.2/onyx_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/handlers.py` & `onyx_extension-0.4.2/onyx_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/build_log.json` & `onyx_extension-0.4.2/onyx_extension/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999993827160494%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'onyx_extension': {'version': '0.4.2'}}}}}}"}*

```diff
@@ -661,15 +661,15 @@
                             "requiredVersion": "^2.49.2",
                             "singleton": true
                         },
                         "climb-onyx-ui": {},
                         "onyx_extension": {
                             "import": "C:\\Users\\butchena\\Documents\\projects\\CLIMB-TRE(FCOD-LOMAN-NJ-1)\\gitlab\\onyx-extension\\lib\\index.js",
                             "singleton": true,
-                            "version": "0.4.1"
+                            "version": "0.4.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/package.json` & `onyx_extension-0.4.2/onyx_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static\\\\remoteEntry.8132ef2cf277548ef51c.js'}}",*

 * * "'version'": "'0.4.2'"}*

```diff
@@ -106,15 +106,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/extension-onyx_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static\\remoteEntry.0fa3b8b49d2409fd11bb.js",
+            "load": "static\\remoteEntry.8132ef2cf277548ef51c.js",
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
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/lib_index_js.4bae6e3d1c04b0e96d5c.js` & `onyx_extension-0.4.2/onyx_extension/labextension/static/lib_index_js.387211c2f04c65e8ccd7.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -80,14 +80,17 @@
                  */
                 async function requestAPI(endPoint = '', init = {}, param = ['', '']) {
                     // Make request to Jupyter API
                     const settings = _jupyterlab_services__WEBPACK_IMPORTED_MODULE_0__.ServerConnection.makeSettings();
                     let url = new URL('/onyx-extension/' + endPoint, settings.baseUrl);
                     if (param[0] != '')
                         url.searchParams.append(param[0], param[1]);
+                    console.log(url.toString());
+                    console.log(settings.baseUrl);
+                    console.log(url.toString().indexOf(settings.baseUrl));
                     let response;
                     try {
                         response = await _jupyterlab_services__WEBPACK_IMPORTED_MODULE_0__.ServerConnection.makeRequest(url.toString(), init, settings);
                     } catch (error) {
                         throw new _jupyterlab_services__WEBPACK_IMPORTED_MODULE_0__.ServerConnection.NetworkError(error);
                     }
                     let data = await response.text();
@@ -286,8 +289,8 @@
                 module.exports = "<svg xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\" version=\"1.1\" width=\"256\" height=\"256\" viewBox=\"0 0 256 256\" xml:space=\"preserve\">\n\n<defs>\n</defs>\n<g style=\"stroke: none; stroke-width: 0; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: none; fill-rule: nonzero; opacity: 1;\" transform=\"translate(1.4065934065934016 1.4065934065934016) scale(2.81 2.81)\" >\n\t<path d=\"M 73.352 33.287 c -1.16 0 -2.35 -0.064 -3.563 -0.193 c -0.824 -0.088 -1.42 -0.827 -1.332 -1.651 c 0.088 -0.825 0.841 -1.413 1.65 -1.333 c 7.211 0.774 13.366 -0.99 17.333 -4.956 c 0.586 -0.586 1.535 -0.586 2.121 0 s 0.586 1.536 0 2.121 C 85.631 31.205 79.962 33.287 73.352 33.287 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 26.214 90 c -0.384 0 -0.768 -0.146 -1.061 -0.439 c -0.586 -0.586 -0.586 -1.535 0 -2.121 c 5.682 -5.683 6.724 -15.295 2.858 -26.374 C 24.045 49.694 24.94 39.392 30.467 32.8 c 4.991 -5.954 13.106 -8.365 22.838 -6.79 c 0.818 0.132 1.374 0.903 1.241 1.721 s -0.907 1.366 -1.72 1.241 c -8.652 -1.401 -15.775 0.645 -20.061 5.755 c -4.831 5.762 -5.531 15.001 -1.92 25.35 c 4.259 12.209 2.958 22.955 -3.57 29.483 C 26.982 89.854 26.598 90 26.214 90 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 42.32 64.459 c -1.732 0 -3.535 -0.144 -5.399 -0.434 c -0.818 -0.128 -1.379 -0.895 -1.251 -1.713 c 0.127 -0.819 0.897 -1.372 1.713 -1.252 c 8.575 1.34 15.636 -0.731 19.881 -5.823 c 4.804 -5.764 5.493 -14.99 1.892 -25.314 c -4.259 -12.21 -2.958 -22.956 3.57 -29.483 c 0.586 -0.586 1.535 -0.586 2.121 0 s 0.586 1.536 0 2.121 c -5.682 5.682 -6.724 15.294 -2.859 26.374 c 3.958 11.344 3.076 21.631 -2.419 28.224 C 55.577 61.946 49.567 64.459 42.32 64.459 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 1.5 65.286 c -0.384 0 -0.768 -0.146 -1.061 -0.439 c -0.586 -0.586 -0.586 -1.535 0 -2.121 c 5.047 -5.047 12.812 -7.013 21.865 -5.536 c 0.817 0.134 1.372 0.904 1.239 1.722 c -0.134 0.818 -0.907 1.372 -1.722 1.239 c -8.073 -1.316 -14.914 0.35 -19.26 4.696 C 2.268 65.14 1.884 65.286 1.5 65.286 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 61.713 51.758 c -0.384 0 -0.768 -0.146 -1.061 -0.439 L 38.685 29.351 c -0.586 -0.585 -0.586 -1.536 0 -2.121 c 0.586 -0.586 1.535 -0.586 2.121 0 l 21.968 21.968 c 0.586 0.586 0.586 1.535 0 2.121 C 62.48 51.611 62.097 51.758 61.713 51.758 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 50.258 63.213 c -0.384 0 -0.768 -0.146 -1.061 -0.439 L 27.229 40.806 c -0.586 -0.585 -0.586 -1.536 0 -2.121 c 0.586 -0.586 1.535 -0.586 2.121 0 l 21.968 21.968 c 0.586 0.586 0.586 1.535 0 2.121 C 51.025 63.066 50.642 63.213 50.258 63.213 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 82.111 31.79 c -0.384 0 -0.768 -0.146 -1.061 -0.439 L 58.646 8.946 c -0.586 -0.585 -0.586 -1.536 0 -2.121 c 0.586 -0.586 1.535 -0.586 2.121 0 l 22.404 22.405 c 0.586 0.585 0.586 1.536 0 2.121 C 82.879 31.644 82.495 31.79 82.111 31.79 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n\t<path d=\"M 29.133 84.769 c -0.384 0 -0.768 -0.146 -1.061 -0.439 L 5.667 61.925 c -0.586 -0.586 -0.586 -1.535 0 -2.121 s 1.535 -0.586 2.121 0 l 22.405 22.404 c 0.586 0.586 0.586 1.535 0 2.121 C 29.9 84.622 29.517 84.769 29.133 84.769 z\" style=\"stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;\" transform=\" matrix(1 0 0 1 0 0) \" stroke-linecap=\"round\" />\n</g>\n</svg>";
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.4bae6e3d1c04b0e96d5c.js.map
+//# sourceMappingURL=lib_index_js.387211c2f04c65e8ccd7.js.map
```

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/lib_index_js.4bae6e3d1c04b0e96d5c.js.map` & `onyx_extension-0.4.2/onyx_extension/labextension/static/lib_index_js.387211c2f04c65e8ccd7.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'lib_index_js.387211c2f04c65e8ccd7.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;AAA0B;AACyB;AACnD,iDAAiD;AAChB;AAE1B,MAAM,cAAe,SAAQ,6DAAW;IAC7C,YAAY,GAAW,EAAE,GAAW;QAClC,KAAK,EAAE,CAAC;QACR,IAAI,CAAC,MAAM,GAAG,GAAG,CAAC;QAClB,IAAI,CAAC,KAAK,GAAG,GAAG,CAAC;IACnB,CAAC;IAKD,MAAM;QACJ,OAAO,2DAAC,sDAAI,IAAC,MAAM,EAAE,IAAI,CAAC,MAAM,EAAE,KAAK,EAAE,IAAI,CAAC,KAAK,GAAI,CAAC;IAC1D,CAAC;CACF;;;;;;;;;;;;;;;;;AClBuD;AAExD;;;;;;GAMG;AACI,KAAK,UAAU,UAAU,CAC9B,QAAQ,GAAG,EAAE,EACb,OAAoB,EAAE,EACtB,QAA0B,CAAC,EAAE, […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.4bae6e3d1c04b0e96d5c.js",
-    "mappings": "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",
+    "file": "lib_index_js.387211c2f04c65e8ccd7.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://onyx_extension/./src/App.tsx",
         "webpack://onyx_extension/./src/handler.ts",
         "webpack://onyx_extension/./src/icon.ts",
         "webpack://onyx_extension/./src/index.ts"
     ],
     "sourcesContent": [
         "import React from 'react';\r\nimport { ReactWidget } from '@jupyterlab/apputils';\r\n//import App from '../../react-prototype/src/App'\r\nimport Onyx from 'climb-onyx-ui';\r\n\r\nexport class ReactAppWidget extends ReactWidget {\r\n  constructor(dom: string, tok: string) {\r\n    super();\r\n    this.domain = dom;\r\n    this.token = tok;\r\n  }\r\n\r\n  domain: string;\r\n  token: string;\r\n\r\n  render(): JSX.Element {\r\n    return <Onyx domain={this.domain} token={this.token} />;\r\n  }\r\n}\r\n",
-        "import { ServerConnection } from '@jupyterlab/services';\n\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI<T>(\n  endPoint = '',\n  init: RequestInit = {},\n  param: [string, string] = ['', '']\n): Promise<T> {\n  // Make request to Jupyter API\n  const settings = ServerConnection.makeSettings();\n\n  let url = new URL('/onyx-extension/' + endPoint, settings.baseUrl);\n  if (param[0] != '') url.searchParams.append(param[0], param[1]);\n\n  let response: Response;\n  try {\n    response = await ServerConnection.makeRequest(\n      url.toString(),\n      init,\n      settings\n    );\n  } catch (error) {\n    throw new ServerConnection.NetworkError(error as any);\n  }\n\n  let data: any = await response.text();\n\n  if (data.length > 0) {\n    try {\n      data = JSON.parse(data);\n    } catch (error) {\n      console.log('Not a JSON response body.', response);\n    }\n  }\n\n  if (!response.ok) {\n    throw new ServerConnection.ResponseError(response, data.message || data);\n  }\n\n  return data;\n}\n",
+        "import { ServerConnection } from '@jupyterlab/services';\n\n/**\n * Call the API extension\n *\n * @param endPoint API REST end point for the extension\n * @param init Initial values for the request\n * @returns The response body interpreted as JSON\n */\nexport async function requestAPI<T>(\n  endPoint = '',\n  init: RequestInit = {},\n  param: [string, string] = ['', '']\n): Promise<T> {\n  // Make request to Jupyter API\n  const settings = ServerConnection.makeSettings();\n\n  let url = new URL('/onyx-extension/' + endPoint, settings.baseUrl);\n  if (param[0] != '') url.searchParams.append(param[0], param[1]);\n\n  console.log(url.toString())\n  console.log(settings.baseUrl)\n  console.log(url.toString().indexOf(settings.baseUrl))\n\n  let response: Response;\n  try {\n    response = await ServerConnection.makeRequest(\n      url.toString(),\n      init,\n      settings\n    );\n  } catch (error) {\n    throw new ServerConnection.NetworkError(error as any);\n  }\n\n  let data: any = await response.text();\n\n  if (data.length > 0) {\n    try {\n      data = JSON.parse(data);\n    } catch (error) {\n      console.log('Not a JSON response body.', response);\n    }\n  }\n\n  if (!response.ok) {\n    throw new ServerConnection.ResponseError(response, data.message || data);\n  }\n\n  return data;\n}\n",
         "import { LabIcon } from '@jupyterlab/ui-components';\nimport CHAT_ICON from './../style/icons/dna.svg';\n\nexport const chatIcon = new LabIcon({\n  name: 'jitsi:chat',\n  svgstr: CHAT_ICON\n});\n",
         "import {\r\n  JupyterFrontEnd,\r\n  JupyterFrontEndPlugin\r\n} from '@jupyterlab/application';\r\n\r\nimport {\r\n  ICommandPalette,\r\n  MainAreaWidget,\r\n  WidgetTracker\r\n} from '@jupyterlab/apputils';\r\n\r\nimport { IDocumentManager } from '@jupyterlab/docmanager';\r\n\r\nimport { ILauncher } from '@jupyterlab/launcher';\r\n\r\nimport { requestAPI } from './handler';\r\nimport { ReactAppWidget } from './App';\r\nimport { chatIcon } from './icon';\r\n\r\n/**\r\n * Initialization data for the onyx_extension extension.\r\n */\r\nconst plugin: JupyterFrontEndPlugin<void> = {\r\n  id: 'onyx_extension:plugin',\r\n  description: 'Onyx-extension.',\r\n  autoStart: true,\r\n  optional: [ILauncher],\r\n  requires: [ICommandPalette, IDocumentManager],\r\n  activate: (\r\n    app: JupyterFrontEnd,\r\n    palette: ICommandPalette,\r\n    documentManager: IDocumentManager,\r\n    launcher: ILauncher | null\r\n  ) => {\r\n    console.log('JupyterLab extension @onyx_extension is activated!');\r\n\r\n    const command = 'onyx_extension';\r\n    const s3_command = 's3_onyx_extension';\r\n    const category = 'Onyx';\r\n\r\n    let domain: string;\r\n    let token: string;\r\n\r\n    const s3_open_function = (s3_link: string) => {\r\n      requestAPI<any>('s3', {}, ['s3location', s3_link])\r\n        .then(data => {\r\n          console.log(data);\r\n          documentManager.open(data['temp_file']);\r\n        })\r\n        .catch(reason => {\r\n          console.error(\r\n            `The onyx_extension server extension appears to be missing.\\n${reason}`\r\n          );\r\n        });\r\n    };\r\n\r\n    requestAPI<any>('settings')\r\n      .then(data => {\r\n        console.log(data);\r\n        domain = data['domain'];\r\n        token = data['token'];\r\n      })\r\n      .catch(reason => {\r\n        console.error(\r\n          `The onyx_extension server extension appears to be missing.\\n${reason}`\r\n        );\r\n      });\r\n\r\n    // Create a single widget\r\n    let widget: MainAreaWidget<ReactAppWidget>;\r\n\r\n    app.commands.addCommand(command, {\r\n      label: 'Onyx',\r\n      caption: 'Onyx',\r\n      icon: chatIcon,\r\n      execute: () => {\r\n        if (!widget || widget.disposed) {\r\n          const content = new ReactAppWidget(domain, token);\r\n          widget = new MainAreaWidget({ content });\r\n          widget.title.label = 'Onyx';\r\n          widget.title.closable = true;\r\n        }\r\n        if (!tracker.has(widget)) {\r\n          tracker.add(widget);\r\n        }\r\n        if (!widget.isAttached) {\r\n          // Attach the widget to the main work area if it's not there\r\n          app.shell.add(widget, 'main');\r\n        }\r\n\r\n        // Activate the widget\r\n        app.shell.activateById(widget.id);\r\n      }\r\n    });\r\n\r\n    palette.addItem({ command, category: category });\r\n\r\n    if (launcher) {\r\n      // Add launcher\r\n      launcher.add({\r\n        command: command,\r\n        category: category\r\n      });\r\n    }\r\n\r\n    app.commands.addCommand(s3_command, {\r\n      label: 'Onyx s3',\r\n      caption: 'Onyx s3',\r\n      icon: chatIcon,\r\n      execute: () => {\r\n        s3_open_function(\r\n          's3://mscape-published-reports/C-B01922D432_scylla_report.html'\r\n        );\r\n      }\r\n    });\r\n\r\n    palette.addItem({ command: s3_command, category: category });\r\n  }\r\n};\r\n\r\nconst tracker = new WidgetTracker<MainAreaWidget<ReactAppWidget>>({\r\n  namespace: 'onyx_extension'\r\n});\r\n\r\nexport default plugin;\r\n"
     ],
     "version": 3
 }
```

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/remoteEntry.0fa3b8b49d2409fd11bb.js` & `onyx_extension-0.4.2/onyx_extension/labextension/static/remoteEntry.8132ef2cf277548ef51c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -183,15 +183,15 @@
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
                 "webpack_sharing_consume_default_react": "b6171cc67744114369b8",
-                "lib_index_js": "4bae6e3d1c04b0e96d5c",
+                "lib_index_js": "387211c2f04c65e8ccd7",
                 "vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d": "daff3ca64e09afb815f2",
                 "style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9": "e7e279648ddef5dfd55a",
                 "vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js": "32d25ee4ef05954a5218"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -432,15 +432,15 @@
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
                     register("climb-onyx-ui", "0.4.0", () => (Promise.all([__webpack_require__.e("vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js"), __webpack_require__.e("webpack_sharing_consume_default_react")]).then(() => (() => (__webpack_require__( /*! ./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js */ "./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js"))))));
                     /******/
-                    register("onyx_extension", "0.4.1", () => (Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("onyx_extension", "0.4.2", () => (Promise.all([__webpack_require__.e("webpack_sharing_consume_default_react"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1114,8 +1114,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/onyx_extension");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).onyx_extension = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.0fa3b8b49d2409fd11bb.js.map
+//# sourceMappingURL=remoteEntry.8132ef2cf277548ef51c.js.map
```

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/remoteEntry.0fa3b8b49d2409fd11bb.js.map` & `onyx_extension-0.4.2/onyx_extension/labextension/static/remoteEntry.8132ef2cf277548ef51c.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9142857142857144%*

 * *Differences: {"'file'": "'remoteEntry.8132ef2cf277548ef51c.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"webpack_sharing_consume_default_react":"b6171cc67744114369b8","lib_index_js":"387211c2f04c65e8ccd7","vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.0fa3b8b49d2409fd11bb.js",
+    "file": "remoteEntry.8132ef2cf277548ef51c.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,mbAAmb;WACjd;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC9CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WC5LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://onyx_extension/webpack/container-entry",
         "webpack://onyx_extension/webpack/bootstrap",
         "webpack://onyx_extension/webpack/runtime/compat get default export",
@@ -25,20 +25,20 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d\"), __webpack_require__.e(\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"webpack_sharing_consume_default_react\":\"b6171cc67744114369b8\",\"lib_index_js\":\"4bae6e3d1c04b0e96d5c\",\"vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d\":\"daff3ca64e09afb815f2\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9\":\"e7e279648ddef5dfd55a\",\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\":\"32d25ee4ef05954a5218\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"webpack_sharing_consume_default_react\":\"b6171cc67744114369b8\",\"lib_index_js\":\"387211c2f04c65e8ccd7\",\"vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d\":\"daff3ca64e09afb815f2\",\"style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9\":\"e7e279648ddef5dfd55a\",\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\":\"32d25ee4ef05954a5218\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"onyx_extension:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"onyx_extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"climb-onyx-ui\", \"0.4.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js */ \"./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js\"))))));\n\t\t\tregister(\"onyx_extension\", \"0.4.1\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"onyx_extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"climb-onyx-ui\", \"0.4.0\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\"), __webpack_require__.e(\"webpack_sharing_consume_default_react\")]).then(() => (() => (__webpack_require__(/*! ./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js */ \"./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js\"))))));\n\t\t\tregister(\"onyx_extension\", \"0.4.2\", () => (Promise.all([__webpack_require__.e(\"webpack_sharing_consume_default_react\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,18,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/docmanager\", [1,4,1,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,1,8])),\n\t\"webpack/sharing/consume/default/@jupyterlab/services\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/services\", [1,7,1,8])),\n\t\"webpack/sharing/consume/default/climb-onyx-ui/climb-onyx-ui\": () => (loadStrictVersionCheckFallback(\"default\", \"climb-onyx-ui\", [2,0,4,0], () => (__webpack_require__.e(\"vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js\").then(() => (() => (__webpack_require__(/*! climb-onyx-ui */ \"./node_modules/climb-onyx-ui/dist/climb-onyx-ui.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,8]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"webpack_sharing_consume_default_react\": [\n\t\t\"webpack/sharing/consume/default/react\"\n\t],\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docmanager\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/services\",\n\t\t\"webpack/sharing/consume/default/climb-onyx-ui/climb-onyx-ui\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
         "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"onyx_extension\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(\"webpack_sharing_consume_default_react\" != chunkId) {\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkonyx_extension\"] = self[\"webpackChunkonyx_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/onyx_extension\");\n",
         ""
```

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js` & `onyx_extension-0.4.2/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map` & `onyx_extension-0.4.2/onyx_extension/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-92e3d9.e7e279648ddef5dfd55a.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js` & `onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map` & `onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_climb-onyx-ui_dist_climb-onyx-ui_js.32d25ee4ef05954a5218.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js` & `onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map` & `onyx_extension-0.4.2/onyx_extension/labextension/static/vendors-node_modules_style-loader_dist_runtime_injectStylesIntoStyleTag_js-node_modules_style-9a1b2d.daff3ca64e09afb815f2.js.map`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/src/handler.ts` & `onyx_extension-0.4.2/src/handler.ts`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 ): Promise<T> {
   // Make request to Jupyter API
   const settings = ServerConnection.makeSettings();
 
   let url = new URL('/onyx-extension/' + endPoint, settings.baseUrl);
   if (param[0] != '') url.searchParams.append(param[0], param[1]);
 
+  console.log(url.toString())
+  console.log(settings.baseUrl)
+  console.log(url.toString().indexOf(settings.baseUrl))
+
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(
       url.toString(),
       init,
       settings
     );
```

### Comparing `onyx_extension-0.4.1/src/index.ts` & `onyx_extension-0.4.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/style/icons/dna.svg` & `onyx_extension-0.4.2/style/icons/dna.svg`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/.gitignore` & `onyx_extension-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/pyproject.toml` & `onyx_extension-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onyx_extension-0.4.1/PKG-INFO` & `onyx_extension-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: onyx_extension
-Version: 0.4.1
+Version: 0.4.2
 Dynamic: Keywords
 Summary: A minimal JupyterLab extension with backend and frontend parts.
 Project-URL: Homepage, https://github.com/jupyterlab/extension-onyx_extension
 Project-URL: Bug Tracker, https://github.com/jupyterlab/extension-onyx_extension/issues
 Project-URL: Repository, https://github.com/jupyterlab/extension-onyx_extension.git
 Author: Project Jupyter Contributors
 License: MIT
```

