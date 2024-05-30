# Comparing `tmp/gradio_clickabletextbox-0.0.6.tar.gz` & `tmp/gradio_clickabletextbox-0.0.7.tar.gz`

## Comparing `gradio_clickabletextbox-0.0.6.tar` & `gradio_clickabletextbox-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/__init__.py
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.py
--rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.pyi
--rw-r--r--   0        0        0    97509 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/index.js
--rw-r--r--   0        0        0    16635 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/css.css
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/requirements.txt
--rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/Example.svelte
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/Index.svelte
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/gradio.config.js
--rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/package-lock.json
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/package.json
--rw-r--r--   0        0        0    16137 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/shared/Textbox.svelte
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/frontend/shared/transitions.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/.gitignore
--rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/README.md
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/__init__.py
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/clickabletextbox.py
+-rw-r--r--   0        0        0    37561 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/clickabletextbox.pyi
+-rw-r--r--   0        0        0    97507 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/component/index.js
+-rw-r--r--   0        0        0    16635 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/demo/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/demo/css.css
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/demo/requirements.txt
+-rw-r--r--   0        0        0    10461 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/Example.svelte
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/Index.svelte
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/gradio.config.js
+-rw-r--r--   0        0        0   150164 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/package-lock.json
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/package.json
+-rw-r--r--   0        0        0    16135 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/shared/Textbox.svelte
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/frontend/shared/transitions.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/.gitignore
+-rw-r--r--   0        0        0    10662 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/README.md
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 gradio_clickabletextbox-0.0.7/PKG-INFO
```

### Comparing `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.py` & `gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/clickabletextbox.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/clickabletextbox.pyi` & `gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/clickabletextbox.pyi`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/index.js` & `gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/component/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2252,19 +2252,19 @@
     function W() {
         return n(this, void 0, void 0, function*() {
             t(14, T = !T);
         });
     }
 
     function se(d) {
-        i.trim() && t(0, i += ", "), t(0, i += `${d} `);
+        i.trim() && t(0, i += ", "), t(0, i += `${d}`);
     }
 
     function K(d) {
-        t(0, i += `${d} `);
+        t(0, i += `${d}`);
     }
 
     function we(d) {
         const A = d.target,
             O = A.value,
             D = [A.selectionStart, A.selectionEnd];
         I("select", {
```

### Comparing `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/component/style.css` & `gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/backend/gradio_clickabletextbox/templates/example/index.js` & `gradio_clickabletextbox-0.0.7/backend/gradio_clickabletextbox/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/demo/app.py` & `gradio_clickabletextbox-0.0.7/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/demo/css.css` & `gradio_clickabletextbox-0.0.7/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/demo/space.py` & `gradio_clickabletextbox-0.0.7/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/frontend/Example.svelte` & `gradio_clickabletextbox-0.0.7/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/frontend/Index.svelte` & `gradio_clickabletextbox-0.0.7/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/frontend/package-lock.json` & `gradio_clickabletextbox-0.0.7/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/frontend/package.json` & `gradio_clickabletextbox-0.0.7/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/frontend/shared/Textbox.svelte` & `gradio_clickabletextbox-0.0.7/frontend/shared/Textbox.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -84,19 +84,19 @@
 	}
 
 	function addSuffix(word) {
 		// Add a comma and space if the value is not empty
 		if (value.trim()) {
 			value += ", ";
 		}
-		value += `${word} `;
+		value += `${word}`;
 	}
 
 	function loadPrompt(word) {
-		value += `${word} `;
+		value += `${word}`;
 	}
 
 	function handle_select(event: Event): void {
 		const target: HTMLTextAreaElement | HTMLInputElement = event.target as
 			| HTMLTextAreaElement
 			| HTMLInputElement;
 		const text = target.value;
```

### Comparing `gradio_clickabletextbox-0.0.6/frontend/shared/transitions.js` & `gradio_clickabletextbox-0.0.7/frontend/shared/transitions.js`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/README.md` & `gradio_clickabletextbox-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gradio_clickabletextbox-0.0.6/pyproject.toml` & `gradio_clickabletextbox-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_clickabletextbox"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python library for easily interacting with trained machine learning models"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Textbox"]
 # Add dependencies here
```

### Comparing `gradio_clickabletextbox-0.0.6/PKG-INFO` & `gradio_clickabletextbox-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_clickabletextbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python library for easily interacting with trained machine learning models
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: gradio-custom-component,gradio-template-Textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

