# Comparing `tmp/mappyfile-colors-0.4.1.tar.gz` & `tmp/mappyfile_colors-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mappyfile-colors-0.4.1.tar", last modified: Fri Jul  5 08:54:53 2019, max compression
+gzip compressed data, was "mappyfile_colors-1.0.0.tar", last modified: Thu May 30 21:03:37 2024, max compression
```

## Comparing `mappyfile-colors-0.4.1.tar` & `mappyfile_colors-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2019-07-05 08:54:53.000000 mappyfile-colors-0.4.1/
--rw-rw-rw-   0        0        0     1089 2019-02-22 17:10:05.000000 mappyfile-colors-0.4.1/LICENSE
--rw-rw-rw-   0        0        0       36 2018-02-14 14:16:45.000000 mappyfile-colors-0.4.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2019-07-05 08:54:53.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/
--rw-rw-rw-   0        0        0        1 2019-07-05 08:54:52.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2019-07-05 08:54:52.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-02-22 23:31:02.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5578 2019-07-05 08:54:52.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       27 2019-07-05 08:54:52.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/requires.txt
--rw-rw-rw-   0        0        0      442 2019-07-05 08:54:52.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2019-07-05 08:54:52.000000 mappyfile-colors-0.4.1/mappyfile_colors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7188 2019-07-05 07:59:15.000000 mappyfile-colors-0.4.1/mappyfile_colors.py
--rw-rw-rw-   0        0        0     5578 2019-07-05 08:54:53.000000 mappyfile-colors-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3830 2019-07-05 08:54:24.000000 mappyfile-colors-0.4.1/README.rst
--rw-rw-rw-   0        0        0      168 2019-07-05 08:54:53.000000 mappyfile-colors-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1420 2019-02-26 23:17:01.000000 mappyfile-colors-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2019-07-05 08:54:53.000000 mappyfile-colors-0.4.1/tests/
--rw-rw-rw-   0        0        0     5037 2019-02-26 22:52:10.000000 mappyfile-colors-0.4.1/tests/test_colors.py
--rw-rw-rw-   0        0        0     1199 2019-07-04 13:17:35.000000 mappyfile-colors-0.4.1/tests/test_color_factory.py
--rw-rw-rw-   0        0        0      734 2019-03-06 08:37:26.000000 mappyfile-colors-0.4.1/tests/test_example.py
--rw-rw-rw-   0        0        0     2268 2019-02-26 23:02:36.000000 mappyfile-colors-0.4.1/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:03:37.637544 mappyfile_colors-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-30 21:03:37.637544 mappyfile_colors-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:03:37.637544 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-30 21:03:37.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-30 21:03:37.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:03:37.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 21:03:37.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:03:24.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 21:03:37.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 21:03:37.000000 mappyfile_colors-1.0.0/mappyfile_colors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/mappyfile_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 21:03:37.641543 mappyfile_colors-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:03:37.637544 mappyfile_colors-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/tests/test_color_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-30 21:03:13.000000 mappyfile_colors-1.0.0/tests/test_plugin.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mappyfile-colors-0.4.1/LICENSE` & `mappyfile_colors-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mappyfile-colors-0.4.1/mappyfile_colors.py` & `mappyfile_colors-1.0.0/mappyfile_colors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,90 @@
 import itertools
 from mappyfile.transformer import MapfileTransformer, CommentsTransformer, MapfileToDict
 from mappyfile.parser import Parser
 from lark.visitors import v_args
 import webcolors
 from lark.lexer import Token
 
-__version__ = "0.4.1"
+__version__ = "1.0.0"
 
 
 class ConversionType:
     NO_CONVERSION = 0
     TO_RGB = 1
     TO_HEX = 2
 
 
 class ColorToken(Token):
     """
     A token subclass with an additional comment attribute
     to store the color name so it can be accessed
     by the transformer
     """
-    __slots__ = 'comment'
+
+    __slots__ = "comment"
 
 
 def token_to_rgb(t):
     r, g, b = t
     return (r.value, g.value, b.value)
 
 
-def rgb_to_hex_token(rgb, include_color_names):
-
-    hex = webcolors.rgb_to_hex(rgb)
-    return hex_to_token(hex, include_color_names)
-
-
-def hex_to_rgb_token(hex, include_color_names):
-
-    rgb = webcolors.hex_to_rgb(hex)
-    return rgb_to_token(rgb, include_color_names)
-
-
-def rgb_to_token(rgb, include_color_names):
-
-    r, g, b = rgb
-    rgb_token = ColorToken("RGB", [r, g, b])
-    if include_color_names:
-        add_token_comment(rgb_token)
-    return rgb_token
-
-
-def hex_to_token(hex, include_color_names):
-
-    hex_token = ColorToken("HEXCOLOR", hex)
-    if include_color_names:
-        add_token_comment(hex_token)
-    return hex_token
-
-
-def hex_to_name(hex):
-
-    try:
-        name = webcolors.hex_to_name(hex)
-    except ValueError:
-        name = "unnamed"
-    return name
-
-
-def add_token_comment(token):
-
-    if token.type == "RGB":
-        hex = webcolors.rgb_to_hex(token.value)
-    else:
-        assert token.type == "HEXCOLOR"
-        hex = token.value
-
-    token.comment = hex_to_name(hex)
+def rgb_to_hex_token(rgb, include_color_names):
+    hex = webcolors.rgb_to_hex(rgb)
+    return hex_to_token(hex, include_color_names)
+
+
+def hex_to_rgb_token(hex, include_color_names):
+    rgb = webcolors.hex_to_rgb(hex)
+    return rgb_to_token(rgb, include_color_names)
+
+
+def rgb_to_token(rgb, include_color_names):
+    r, g, b = rgb
+    rgb_token = ColorToken("RGB", [r, g, b])
+    if include_color_names:
+        add_token_comment(rgb_token)
+    return rgb_token
+
+
+def hex_to_token(hex, include_color_names):
+    hex_token = ColorToken("HEXCOLOR", hex)
+    if include_color_names:
+        add_token_comment(hex_token)
+    return hex_token
+
+
+def hex_to_name(hex):
+    try:
+        name = webcolors.hex_to_name(hex)
+    except ValueError:
+        name = "unnamed"
+    return name
+
+
+def add_token_comment(token):
+    if token.type == "RGB":
+        hex = webcolors.rgb_to_hex(token.value)
+    else:
+        assert token.type == "HEXCOLOR"
+        hex = token.value
+
+    token.comment = hex_to_name(hex)
     return token
 
 
 orig_function = CommentsTransformer._save_attr_comments
 
 
 @v_args(tree=True)
 def attr_comments_override(self, tree):
-    """
-    Override the standard comments function to check for any ColorTokens and
-    add the human named colors to the comments array associated with the color
+    """
+    Override the standard comments function to check for any ColorTokens and
+    add the human named colors to the comments array associated with the color
     """
 
     d = orig_function(self, tree)
     if "__tokens__" in d:
         for t in d["__tokens__"]:
             if isinstance(t, ColorToken) and hasattr(t, "comment"):
                 # append the comment to the comments list if not already present
@@ -105,17 +100,22 @@
 
 
 class ColorsTransformer(MapfileTransformer):
     """
     A custom transformer that can convert from RGB to HEX color
     formats, and add in the color name as a comment
     """
-    def __init__(self, include_position=False, include_comments=False,
-                 conversion_type=ConversionType.TO_RGB, include_color_names=False):
 
+    def __init__(
+        self,
+        include_position=False,
+        include_comments=False,
+        conversion_type=ConversionType.TO_RGB,
+        include_color_names=False,
+    ):
         self.conversion_type = conversion_type
 
         if include_color_names is True:
             include_comments = True
 
         self.include_color_names = include_color_names
 
@@ -126,48 +126,48 @@
         Convert rgb values to hex if appropriate, if not
         return the standard transformation
         """
 
         rgb = token_to_rgb(t)
 
         if self.conversion_type == ConversionType.TO_HEX:
-            hex_token = rgb_to_hex_token(rgb, self.include_color_names)
+            hex_token = rgb_to_hex_token(rgb, self.include_color_names)
             return hex_token
         else:
             return rgb_to_token(rgb, self.include_color_names)
 
     def hexcolor(self, t):
         """
         Convert hex values to rgb if appropriate, if not
         return the standard transformation
         """
 
-        hex = self.clean_string(t[0])
+        hex = self.clean_string(t[0].value)
 
-        if self.conversion_type == ConversionType.TO_RGB:
-            rgb_token = hex_to_rgb_token(hex, self.include_color_names)
-            return rgb_token
-        else:
+        if self.conversion_type == ConversionType.TO_RGB:
+            rgb_token = hex_to_rgb_token(hex, self.include_color_names)
+            return rgb_token
+        else:
             return hex_to_token(hex, self.include_color_names)
 
     def colorrange(self, t):
         """
         Convert a rgb colorange to a hex colorrange
 
-        Input is [Token(SIGNED_INT, 0), Token(SIGNED_INT, 0), Token(SIGNED_INT, 0),
+        Input is [Token(SIGNED_INT, 0), Token(SIGNED_INT, 0), Token(SIGNED_INT, 0),
         Token(SIGNED_INT, 255), Token(SIGNED_INT, 255), Token(SIGNED_INT, 255)]
         """
-
-        if self.conversion_type == ConversionType.TO_RGB:
-            return super(ColorsTransformer, self).colorrange(t)
-        else:
-            t1 = t[:3]
-            t2 = t[3:]
-            hex_token1 = rgb_to_hex_token(token_to_rgb(t1), self.include_color_names)
-            hex_token2 = rgb_to_hex_token(token_to_rgb(t2), self.include_color_names)
+
+        if self.conversion_type == ConversionType.TO_RGB:
+            return super(ColorsTransformer, self).colorrange(t)
+        else:
+            t1 = t[:3]
+            t2 = t[3:]
+            hex_token1 = rgb_to_hex_token(token_to_rgb(t1), self.include_color_names)
+            hex_token2 = rgb_to_hex_token(token_to_rgb(t2), self.include_color_names)
             return [hex_token1, hex_token2]
 
     def hexcolorrange(self, t):
         """
         Convert a hex colorange to a rgb colorrange
         """
 
@@ -175,70 +175,115 @@
             r1, g1, b1 = t[0].value  # t[0].comment
             r2, g2, b2 = t[1].value
 
             # TODO why can't 2 RGB values simply be returned here?
 
             # Input is [Token(RGB, [0, 0, 0]), Token(RGB, [255, 255, 255])]
 
-            # colorrange rule expects [Token(SIGNED_INT, 0), Token(SIGNED_INT, 0), Token(SIGNED_INT, 0),
+            # colorrange rule expects [Token(SIGNED_INT, 0), Token(SIGNED_INT, 0), Token(SIGNED_INT, 0),
             # Token(SIGNED_INT, 255), Token(SIGNED_INT, 255), Token(SIGNED_INT, 0)]
 
-            return [Token("SIGNED_INT", r1), Token("SIGNED_INT", g1), Token("SIGNED_INT", b1),
-                    Token("SIGNED_INT", r2), Token("SIGNED_INT", g2), Token("SIGNED_INT", b2)]
+            return [
+                Token("SIGNED_INT", r1),
+                Token("SIGNED_INT", g1),
+                Token("SIGNED_INT", b1),
+                Token("SIGNED_INT", r2),
+                Token("SIGNED_INT", g2),
+                Token("SIGNED_INT", b2),
+            ]
         else:
             return super(ColorsTransformer, self).hexcolorrange(t)
 
 
-def colors_transform(s, conversion_type=ConversionType.NO_CONVERSION, include_comments=False,
-                     include_color_names=False):
+def colors_transform(
+    s,
+    conversion_type=ConversionType.NO_CONVERSION,
+    include_comments=False,
+    include_color_names=False,
+):
     """
     Parse the string with a custom colors transformer
     """
 
     p = Parser(include_comments=include_comments)
     ast = p.parse(s)
 
     if include_color_names:
         include_comments = True
 
-    m = MapfileToDict(include_comments=include_comments,
-                      transformerClass=ColorsTransformer,
-                      conversion_type=conversion_type,
-                      include_color_names=include_color_names)
+    m = MapfileToDict(
+        include_comments=include_comments,
+        transformer_class=ColorsTransformer,
+        conversion_type=conversion_type,
+        include_color_names=include_color_names,
+    )
 
     d = m.transform(ast)
 
     return d
 
 
 class ColorFactory:
-
     palettes = {
         # http://artshacker.com/wp-content/uploads/2014/12/Kellys-22-colour-chart.jpg
-        "maximum_contrast": ['#e6194b', '#3cb44b', '#ffe119', '#4363d8',
-                             '#f58231', '#911eb4', '#46f0f0', '#f032e6',
-                             '#bcf60c', '#fabebe', '#008080', '#e6beff',
-                             '#9a6324', '#fffac8', '#800000', '#aaffc3',
-                             '#808000', '#ffd8b1', '#000075', '#808080',
-                             '#ffffff', '#000000']
+        "maximum_contrast": [
+            "#e6194b",
+            "#3cb44b",
+            "#ffe119",
+            "#4363d8",
+            "#f58231",
+            "#911eb4",
+            "#46f0f0",
+            "#f032e6",
+            "#bcf60c",
+            "#fabebe",
+            "#008080",
+            "#e6beff",
+            "#9a6324",
+            "#fffac8",
+            "#800000",
+            "#aaffc3",
+            "#808000",
+            "#ffd8b1",
+            "#000075",
+            "#808080",
+            "#ffffff",
+            "#000000",
+        ]
     }
 
     def get_colors(self, palette_name=None, repeat=False):
-
         if palette_name is None:
             palette_name = "maximum_contrast"
 
         palette_name = palette_name.lower()
         colours = self.palettes[palette_name]
 
         if repeat:
             colours = itertools.cycle(colours)
 
         for clr in colours:
             yield clr
 
+    def get_gradient_colors(self, rgb1, rgb2, steps):
+        colours = []
+
+        r1, g1, b1 = rgb1
+        r2, g2, b2 = rgb2
+
+        rdelta, gdelta, bdelta = (r2 - r1) / steps, (g2 - g1) / steps, (b2 - b1) / steps
+
+        for step in range(steps):
+            r1 += rdelta
+            g1 += gdelta
+            b1 += bdelta
+            colours.append((r1, g1, b1))
+
+        for clr in colours:
+            yield clr
+
     @property
     def palette_names(self):
         """
         A list of all palette names available in the factory
         """
         return sorted(self.palettes.keys())
```

### Comparing `mappyfile-colors-0.4.1/README.rst` & `mappyfile_colors-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
 + ``include_color_names`` - set to True to add color names as comments (default is False)
 + ``conversion_type`` - a parameter to convert colors within a Mapfile, either import ``ConversionType`` or use an integer value
   to set the conversion:
 
   .. code-block:: python
 
-      NO_CONVERSION = 0
-      TO_RGB = 1
-      TO_HEX = 2
+      NO_CONVERSION = 0
+      TO_RGB = 1
+      TO_HEX = 2
 
 A sample script to convert RGB to HEX colors, and include the color names is shown below. 
 
 .. code-block:: python
 
     import mappyfile
     from mappyfile.plugins import mappyfile_colors 
@@ -68,15 +68,15 @@
             COLOR 184 134 11
             OUTLINECOLOR 0 0 255
             WIDTH 3
         END
     END
     """
 
-    d = mappyfile.loads(s, include_color_names=True, transformerClass=ColorsTransformer, conversion_type=ConversionType.TO_HEX)
+    d = mappyfile.loads(s, include_color_names=True, transformer_class=ColorsTransformer, conversion_type=ConversionType.TO_HEX)
     print(mappyfile.dumps(d))
 
 This will output the following:
 
 .. code-block:: bat
 
     CLASS
```

### Comparing `mappyfile-colors-0.4.1/tests/test_colors.py` & `mappyfile_colors-1.0.0/tests/test_colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 def test_add_rgb_comment():
     s = """
     STYLE
         COLOR 255 0 0
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_HEX, include_color_names=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_HEX, include_color_names=True
+    )
     jsn = json.dumps(d, indent=4)
     print(jsn)
     assert d["__comments__"]["color"][0] == "# red"
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     print(s)
     exp = """STYLE
@@ -65,15 +67,17 @@
 def test_add_hex_comment():
     s = """
     STYLE
         COLOR "#ff0000"
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_RGB, include_color_names=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_RGB, include_color_names=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     exp = """STYLE
 COLOR 255 0 0 # red
 END"""
 
     assert s == exp
@@ -82,15 +86,17 @@
 def test_add_comment_no_conversion():
     s = """
     STYLE
         COLOR "#ff0000"
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.NO_CONVERSION, include_color_names=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.NO_CONVERSION, include_color_names=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     exp = """STYLE
 COLOR '#ff0000' # red
 END"""
 
     print(s)
@@ -100,15 +106,17 @@
 def test_add_comment_no_conversion_rgb():
     s = """
     STYLE
         COLOR 255 0 0
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.NO_CONVERSION, include_color_names=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.NO_CONVERSION, include_color_names=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     exp = """STYLE
 COLOR 255 0 0 # red
 END"""
 
     print(s)
@@ -118,15 +126,17 @@
 def test_add_rgb_colorrange_comment():
     s = """
     STYLE
         COLORRANGE 0 0 0 255 255 255
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_HEX, include_color_names=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_HEX, include_color_names=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     print(s)
     exp = """STYLE
 COLORRANGE '#000000' '#ffffff' # black # white
 END"""
 
@@ -140,15 +150,17 @@
     """
     s = """
     STYLE
         COLORRANGE '#000000' '#ffffff'
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_RGB, include_color_names=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_RGB, include_color_names=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     print(s)
     exp = """STYLE
 COLORRANGE 0 0 0 255 255 255 # black # white
 END"""
 
@@ -158,15 +170,17 @@
 def test_add_to_existing_comments():
     s = """
     STYLE
         COLOR 255 0 0 # my color
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_HEX, include_color_names=True, include_comments=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_HEX, include_color_names=True, include_comments=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     print(s)
     exp = """STYLE
 COLOR '#ff0000' # my color # red
 END"""
 
@@ -179,15 +193,17 @@
     """
     s = """
     STYLE
         COLOR 255 0 0 # my color
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_HEX, include_color_names=True, include_comments=False)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_HEX, include_color_names=True, include_comments=False
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     print(s)
     exp = """STYLE
 COLOR '#ff0000' # red
 END"""
 
@@ -200,15 +216,17 @@
     """
     s = """
     STYLE
         COLOR '#ff0000' # red
     END
     """
 
-    d = mappyfile_colors.colors_transform(s, ConversionType.TO_HEX, include_color_names=True, include_comments=True)
+    d = mappyfile_colors.colors_transform(
+        s, ConversionType.TO_HEX, include_color_names=True, include_comments=True
+    )
     pp = PrettyPrinter(indent=0, quote="'")
     s = pp.pprint(d)
     print(s)
 
     exp = """STYLE
 COLOR '#ff0000' # red
 END"""
@@ -216,12 +234,12 @@
     assert s == exp
 
 
 def run_tests():
     pytest.main(["tests/test_colors.py", "-vv"])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # test_avoid_adding_colorname_twice()
-    test_add_comment_no_conversion_rgb()
-    run_tests()
+    test_to_rgb()
+    # run_tests()
     print("Done!")
```

### Comparing `mappyfile-colors-0.4.1/tests/test_color_factory.py` & `mappyfile_colors-1.0.0/tests/test_color_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import mappyfile_colors
 import pytest
 
 
 def test_get_colors():
-
     color_factory = mappyfile_colors.ColorFactory()
     palette_name = "maximum_contrast"
     clrs = color_factory.get_colors(palette_name)
 
     for c in clrs:
         print(c, mappyfile_colors.hex_to_name(c))
 
@@ -18,38 +17,36 @@
     except StopIteration:
         raised = True
 
     assert raised
 
 
 def test_get_infinite_colors():
-
     color_factory = mappyfile_colors.ColorFactory()
     palette_name = "maximum_contrast"
     clrs = color_factory.get_colors(palette_name, repeat=True)
     # print(list(clrs))  # Don't ever do this with repeat=True!
 
     for i, c in enumerate(clrs):
         print(i, c)
         if i == 100:
             break
 
     assert i == 100
 
 
 def test_get_palette_names():
-
     color_factory = mappyfile_colors.ColorFactory()
     palette_names = color_factory.palette_names
     assert len(palette_names) > 0
 
 
 def run_tests():
     pytest.main(["tests/test_color_factory.py", "-vv"])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     test_get_colors()
     test_get_infinite_colors()
     test_get_palette_names()
     run_tests()
     print("Done!")
```

### Comparing `mappyfile-colors-0.4.1/tests/test_example.py` & `mappyfile_colors-1.0.0/tests/test_example.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 """
 Test the example on the README page
 """
 
 
 def test_example():
-
     import mappyfile
+
     # from mappyfile.plugins import mappyfile_colors
     from mappyfile_colors import ColorsTransformer, ConversionType
 
     s = """
     CLASS
         STYLE
             COLOR 184 134 11
             OUTLINECOLOR 0 0 255
             WIDTH 3
         END
     END
     """
 
-    d = mappyfile.loads(s, include_color_names=True, transformerClass=ColorsTransformer,
-                        conversion_type=ConversionType.TO_HEX)
+    d = mappyfile.loads(
+        s,
+        include_color_names=True,
+        transformer_class=ColorsTransformer,
+        conversion_type=ConversionType.TO_HEX,
+    )
     print(mappyfile.dumps(d))
 
     s = mappyfile.dumps(d)
-    assert s == """CLASS
-    STYLE
-        COLOR "#b8860b"
-        OUTLINECOLOR "#0000ff"
-        WIDTH 3
-    END
+    assert (
+        s
+        == """CLASS
+    STYLE
+        COLOR "#b8860b"
+        OUTLINECOLOR "#0000ff"
+        WIDTH 3
+    END
 END"""
+    )
 
 
 test_example()
```

### Comparing `mappyfile-colors-0.4.1/tests/test_plugin.py` & `mappyfile_colors-1.0.0/tests/test_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,77 +3,95 @@
 from mappyfile_colors import ColorsTransformer, ConversionType
 from mappyfile.parser import Parser
 from mappyfile.transformer import MapfileToDict
 from mappyfile.pprint import PrettyPrinter
 
 
 def test_simple_api():
-
     s = """
     CLASS
         STYLE
             COLOR 184 134 11
             OUTLINECOLOR 0 0 255
             WIDTH 3
         END
     END
     """
 
-    d = mappyfile.loads(s, include_color_names=True, include_comments=True, transformerClass=ColorsTransformer,
-                        conversion_type=ConversionType.TO_HEX)
+    d = mappyfile.loads(
+        s,
+        include_color_names=True,
+        include_comments=True,
+        transformer_class=ColorsTransformer,
+        conversion_type=ConversionType.TO_HEX,
+    )
     output = mappyfile.dumps(d, indent=0, newlinechar=" ")
-    assert output == 'CLASS STYLE COLOR "#b8860b" # darkgoldenrod OUTLINECOLOR "#0000ff" # blue WIDTH 3 END END'
+    assert (
+        output
+        == 'CLASS STYLE COLOR "#b8860b" # darkgoldenrod OUTLINECOLOR "#0000ff" # blue WIDTH 3 END END'
+    )
 
 
 def test_simple_api_rgb():
-
     s = """
     CLASS
         STYLE
             COLOR "#b8860b"
             OUTLINECOLOR "#0000ff"
             WIDTH 3
         END
     END
     """
 
-    d = mappyfile.loads(s, include_color_names=True, include_comments=True, transformerClass=ColorsTransformer,
-                        conversion_type=ConversionType.TO_RGB)
+    d = mappyfile.loads(
+        s,
+        include_color_names=True,
+        include_comments=True,
+        transformer_class=ColorsTransformer,
+        conversion_type=ConversionType.TO_RGB,
+    )
     output = mappyfile.dumps(d, indent=0, newlinechar=" ")
     print(output)
-    assert output == 'CLASS STYLE COLOR 184 134 11 # darkgoldenrod OUTLINECOLOR 0 0 255 # blue WIDTH 3 END END'
+    assert (
+        output
+        == "CLASS STYLE COLOR 184 134 11 # darkgoldenrod OUTLINECOLOR 0 0 255 # blue WIDTH 3 END END"
+    )
 
 
 def test_api():
-
     s = """
     CLASS
         STYLE
             COLOR 184 134 11
             OUTLINECOLOR 0 0 255
             WIDTH 3 # ignore this comment
         END
     END
     """
 
     p = Parser(expand_includes=True, include_comments=False)
     ast = p.parse(s)
 
-    m = MapfileToDict(include_comments=True,
-                      include_color_names=True,  # if this is True then include_comments must also be true
-                      transformerClass=ColorsTransformer,
-                      conversion_type=ConversionType.TO_HEX)
+    m = MapfileToDict(
+        include_comments=True,
+        include_color_names=True,  # if this is True then include_comments must also be true
+        transformer_class=ColorsTransformer,
+        conversion_type=ConversionType.TO_HEX,
+    )
 
     d = m.transform(ast)
     pp = PrettyPrinter(indent=0, newlinechar=" ")
     output = pp.pprint(d)
-    assert output == 'CLASS STYLE COLOR "#b8860b" # darkgoldenrod OUTLINECOLOR "#0000ff" # blue WIDTH 3 END END'
+    assert (
+        output
+        == 'CLASS STYLE COLOR "#b8860b" # darkgoldenrod OUTLINECOLOR "#0000ff" # blue WIDTH 3 END END'
+    )
 
 
 def run_tests():
     pytest.main(["tests/test_plugin.py", "-vv"])
 
 
-if __name__ == '__main__':
-    test_api()
-    # run_tests()
+if __name__ == "__main__":
+    # test_api()
+    run_tests()
     print("Done!")
```

