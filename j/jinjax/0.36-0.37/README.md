# Comparing `tmp/jinjax-0.36.tar.gz` & `tmp/jinjax-0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjax-0.36.tar", max compression
+gzip compressed data, was "jinjax-0.37.tar", max compression
```

## Comparing `jinjax-0.36.tar` & `jinjax-0.37.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      497 2024-05-07 20:49:16.440922 jinjax-0.36/README.md
--rw-r--r--   0        0        0     3839 2024-05-07 20:49:16.448922 jinjax-0.36/pyproject.toml
--rw-r--r--   0        0        0      189 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/__init__.py
--rw-r--r--   0        0        0    13752 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/catalog.py
--rw-r--r--   0        0        0     6897 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/component.py
--rw-r--r--   0        0        0      409 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/exceptions.py
--rw-r--r--   0        0        0     5289 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/html_attrs.py
--rw-r--r--   0        0        0     4657 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/jinjax.py
--rw-r--r--   0        0        0     1304 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/middleware.py
--rw-r--r--   0        0        0        0 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/py.typed
--rw-r--r--   0        0        0       83 2024-05-07 20:49:16.448922 jinjax-0.36/src/jinjax/utils.py
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.36/PKG-INFO
+-rw-r--r--   0        0        0      497 2024-05-29 22:17:26.224059 jinjax-0.37/README.md
+-rw-r--r--   0        0        0     3839 2024-05-29 22:17:26.232060 jinjax-0.37/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/__init__.py
+-rw-r--r--   0        0        0    13750 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/catalog.py
+-rw-r--r--   0        0        0     6917 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/component.py
+-rw-r--r--   0        0        0      409 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/exceptions.py
+-rw-r--r--   0        0        0     5376 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/html_attrs.py
+-rw-r--r--   0        0        0     4665 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/jinjax.py
+-rw-r--r--   0        0        0     1304 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/py.typed
+-rw-r--r--   0        0        0       83 2024-05-29 22:17:26.232060 jinjax-0.37/src/jinjax/utils.py
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 jinjax-0.37/PKG-INFO
```

### Comparing `jinjax-0.36/pyproject.toml` & `jinjax-0.37/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jinjax"
-version = "0.36"
+version = "0.37"
 description = "Replace your HTML templates with Python server-Side components"
 authors = ["Juan-Pablo Scaletti <juanpablo@jpscaletti.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://jinjax.scaletti.dev/"
 repository = "https://github.com/jpsca/jinjax"
 documentation = "https://jinjax.scaletti.dev/guides/"
```

### Comparing `jinjax-0.36/src/jinjax/catalog.py` & `jinjax-0.37/src/jinjax/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
         caller: "t.Callable | None" = None,
         **kw,
     ) -> str:
         content = (kw.pop("__content", "") or "").strip()
         attrs = kw.pop("__attrs", None) or {}
         file_ext = kw.pop("__file_ext", "")
         source = kw.pop("__source", "")
-
         prefix, name = self._split_name(__name)
         url_prefix = self._get_url_prefix(prefix)
         self.jinja_env.loader = self.prefixes[prefix]
 
         if source:
             logger.debug("Rendering from source %s", __name)
             component = self._get_from_source(
@@ -231,15 +230,14 @@
 
             if url not in self.collected_js:
                 self.collected_js.append(url)
 
         attrs = attrs.as_dict if isinstance(attrs, HTMLAttrs) else attrs
         attrs.update(kw)
         kw = attrs
-
         props, extra = component.filter_args(kw)
         try:
             props[PROP_ATTRS] = HTMLAttrs(extra)
         except Exception as exc:
             raise InvalidArgument(
                 f"The arguments of the component <{component.name}>"
                 f"were parsed incorrectly as:\n {str(kw)}"
```

### Comparing `jinjax-0.36/src/jinjax/component.py` & `jinjax-0.37/src/jinjax/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,11 +224,12 @@
         for key in self.optional:
             props[key] = kw.pop(key, self.optional[key])
         extra = kw.copy()
         return props, extra
 
     def render(self, **kwargs):
         assert self.tmpl, f"Component {self.name} has no template"
-        return Markup(self.tmpl.render(**kwargs).strip())
+        html = self.tmpl.render(**kwargs).strip()
+        return Markup(html)
 
     def __repr__(self) -> str:
         return f'<Component "{self.name}">'
```

### Comparing `jinjax-0.36/src/jinjax/html_attrs.py` & `jinjax-0.37/src/jinjax/html_attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         ]))
         self.__classes = {name for name in class_names if name}
 
         for name, value in attrs.items():
             name = name.replace("_", "-")
             if value is True:
                 properties.add(name)
-            elif value not in (False, None):
+            elif value is not False and value is not None:
                 attributes[name] = LazyString(value)
 
         self.__attributes = attributes
         self.__properties = properties
 
     @property
     def classes(self) -> str:
@@ -79,27 +79,30 @@
 
     def __getitem__(self, name: str) -> Any:
         return self.get(name)
 
     def __delitem__(self, name: str) -> None:
         self._remove(name)
 
+    def __str__(self) -> str:
+        return str(self.as_dict)
+
     def set(self, **kw) -> None:
         """
         Sets an attribute or property:
         - Pass a name and a value to set an attribute
         - Use `True` as value to set a property
         - Use `False` to remove an attribute or property
 
         If the attribute is "class", the new classes are appended to
         the old ones instead of replacing them.
         """
         for name, value in kw.items():
             name = name.replace("_", "-")
-            if value in (False, None):
+            if value is False or value is None:
                 self._remove(name)
                 continue
 
             if name in CLASS_KEYS:
                 self.add_class(value)
             elif value is True:
                 self.__properties.add(name)
```

### Comparing `jinjax-0.36/src/jinjax/jinjax.py` & `jinjax-0.37/src/jinjax/jinjax.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 ATTR_END = "}"
 re_attr_name = r""
 re_equal = r""
 re_attr = r"""
 (?P<name>[a-zA-Z@:$_][a-zA-Z@:$_0-9-]*)
 (?:
     \s*=\s*
-    (?P<value>".*?"|'.*?'|\{.*?\})
+    (?P<value>".*?"|'.*?'|\{\s*.*?\s*\})
 )?
-(?:\s+|/|$)
+(?:\s+|/|"|$)
 """
 RX_ATTR = re.compile(re_attr, re.VERBOSE | re.DOTALL)
 
 
 class JinjaX(Extension):
     def preprocess(
         self,
```

### Comparing `jinjax-0.36/src/jinjax/middleware.py` & `jinjax-0.37/src/jinjax/middleware.py`

 * *Files identical despite different names*

### Comparing `jinjax-0.36/PKG-INFO` & `jinjax-0.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjax
-Version: 0.36
+Version: 0.37
 Summary: Replace your HTML templates with Python server-Side components
 Home-page: https://jinjax.scaletti.dev/
 License: MIT
 Author: Juan-Pablo Scaletti
 Author-email: juanpablo@jpscaletti.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

