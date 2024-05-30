# Comparing `tmp/textual_autocomplete-2.1.0b0.tar.gz` & `tmp/textual_autocomplete-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual_autocomplete-2.1.0b0.tar", max compression
+gzip compressed data, was "textual_autocomplete-3.0.0a0.tar", max compression
```

## Comparing `textual_autocomplete-2.1.0b0.tar` & `textual_autocomplete-3.0.0a0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     5108 2023-03-27 15:19:22.966259 textual_autocomplete-2.1.0b0/README.md
--rw-r--r--   0        0        0      721 2023-03-28 09:53:05.687234 textual_autocomplete-2.1.0b0/pyproject.toml
--rw-r--r--   0        0        0      237 2023-03-27 15:19:22.968762 textual_autocomplete-2.1.0b0/textual_autocomplete/__init__.py
--rw-r--r--   0        0        0    19095 2023-03-28 09:52:16.415598 textual_autocomplete-2.1.0b0/textual_autocomplete/_autocomplete.py
--rw-r--r--   0        0        0        0 2022-11-22 11:10:31.804346 textual_autocomplete-2.1.0b0/textual_autocomplete/py.typed
--rw-r--r--   0        0        0     5943 1970-01-01 00:00:00.000000 textual_autocomplete-2.1.0b0/setup.py
--rw-r--r--   0        0        0     5703 1970-01-01 00:00:00.000000 textual_autocomplete-2.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 10:33:52.764840 textual_autocomplete-3.0.0a0/LICENSE
+-rw-r--r--   0        0        0     5108 2024-05-11 10:33:52.766486 textual_autocomplete-3.0.0a0/README.md
+-rw-r--r--   0        0        0      689 2024-05-30 19:19:42.586863 textual_autocomplete-3.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      296 2024-05-29 12:50:02.250077 textual_autocomplete-3.0.0a0/textual_autocomplete/__init__.py
+-rw-r--r--   0        0        0    18968 2024-05-29 23:18:44.386489 textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete.py
+-rw-r--r--   0        0        0    15880 2024-05-30 19:19:06.338711 textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete2.py
+-rw-r--r--   0        0        0        0 2022-11-23 09:28:07.225383 textual_autocomplete-3.0.0a0/textual_autocomplete/py.typed
+-rw-r--r--   0        0        0     5750 1970-01-01 00:00:00.000000 textual_autocomplete-3.0.0a0/PKG-INFO
```

### Comparing `textual_autocomplete-2.1.0b0/README.md` & `textual_autocomplete-3.0.0a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # textual-autocomplete
 
 textual-autocomplete is a Python library for creating dropdown autocompletion menus in
 Textual applications, allowing users to quickly select from a list of suggestions as
-they type. *textual-autocomplete supports **Textual version 0.11.0** and above.*
+they type. *textual-autocomplete supports **Textual version 0.14.0** and above.*
 
 <img width="554" alt="image" src="https://user-images.githubusercontent.com/5740731/205718538-5599a9db-48a2-49dd-99c3-34d43459b81a.png">
 
 <details>
 <summary>Video example</summary>
 
 https://user-images.githubusercontent.com/5740731/205718330-a9364894-9133-40ca-8249-6e3dcc13f456.mov
```

### Comparing `textual_autocomplete-2.1.0b0/pyproject.toml` & `textual_autocomplete-3.0.0a0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "textual-autocomplete"
-version = "2.1.0b0"
+version = "3.0.0a0"
 description = "Easily add autocomplete dropdowns to your Textual apps."
 authors = ["Darren Burns <darrenb900@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "textual_autocomplete" }]
 
 [tool.poetry.dependencies]
-python = "^3.7.8"
+python = "^3.8"
 #textual = {path="../textual", develop=true}
-textual = ">=0.14.0"
+textual = ">=0.58.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 black = "^22.10.0"
-#textual = { version = "^0.10.0", extras = ["dev"] }
-textual = { version = ">=0.14.0", extras = ["dev"] }
+textual = { version = ">=0.58.1", extras = ["dev"] }
 ward = { version = "^0.67.2b0", allow-prereleases = true }
+textual-dev = "^1.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `textual_autocomplete-2.1.0b0/textual_autocomplete/_autocomplete.py` & `textual_autocomplete-3.0.0a0/textual_autocomplete/_autocomplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Callable, ClassVar, Iterable, Mapping, cast
+from typing import Callable, ClassVar, Iterable, Literal, Mapping, cast
 
 from rich.console import Console, ConsoleOptions, RenderableType, RenderResult
 from rich.style import Style
 from rich.table import Table
 from rich.text import Text, TextType
 from textual import events
 from textual.app import ComposeResult
@@ -123,22 +123,24 @@
 @dataclass
 class InputState:
     value: str
     cursor_position: int
 
 
 CompletionStrategy = (
-    "Literal['append', 'replace', 'insert'] | Callable[[str, InputState], InputState]"
+    'Literal["append", "replace", "insert"] | Callable[[str, InputState], InputState]'
 )
 
 
 class AutoComplete(Widget):
     DEFAULT_CSS = """\
 AutoComplete {
     align-horizontal: center;
+    width: auto;
+    height: auto;
 }
     """
 
     def __init__(
         self,
         input: Input,
         dropdown: Dropdown,
@@ -233,36 +235,32 @@
                         cursor_position=self.input.cursor_position,
                     ),
                 )
                 self.input.value = new_state.value
                 self.input.cursor_position = new_state.cursor_position
 
             self.dropdown.display = False
-            self.post_message(
-                self.Selected(item=self.dropdown.selected_item)
-            )
+            self.post_message(self.Selected(item=self.dropdown.selected_item))
 
     class Selected(Message):
         def __init__(self, item: DropdownItem):
             super().__init__()
             self.item = item
 
 
 class Dropdown(Widget):
     DEFAULT_CSS = """\
 Dropdown {
     layer: textual-autocomplete;
-    /* to prevent parent `align` confusing things, we dock to remove from flow */
-    dock: top;
     display: none;
     overflow: hidden auto;
     background: $panel-lighten-1;
     height: auto;
+    width: auto;
     max-height: 12;
-    max-width: 1fr;
     scrollbar-size-vertical: 1;
 }
 
 Dropdown .autocomplete--highlight-match {
     color: $accent-lighten-2;
     text-style: bold;
 }
@@ -315,15 +313,14 @@
         yield self.child
 
     def on_mount(self, event: events.Mount) -> None:
         screen_layers = list(self.screen.styles.layers)
         if not "textual-autocomplete" in screen_layers:
             screen_layers.append("textual-autocomplete")
 
-        # TODO: Ignoring type below because Textual is typed incorrectly here.
         #  Style property setter for layers has incorrect type.
         self.screen.styles.layers = tuple(screen_layers)  # type: ignore
 
         # TODO: Error cases - Handle case where reference to input widget no
         #  longer exists, for example
 
         self.watch(
@@ -405,15 +402,15 @@
                 .plain.lower()
                 .startswith(value.lower()),
             )
 
         self.child.matches = matches
         self.display = len(matches) > 0 and value != "" and self.input_widget.has_focus
         self.cursor_home()
-        self.reposition(input_cursor_position)
+        self.styles.margin = self.input_widget.cursor_screen_offset
         self.child.refresh()
 
     def handle_screen_scroll(self, old: float, new: float) -> None:
         self.reposition(scroll_target_adjust_y=int(old) - int(new))
 
     def reposition(
         self,
@@ -444,14 +441,15 @@
 class DropdownChild(Widget):
     """An autocompletion dropdown widget. This widget gets linked to an Input widget, and is automatically
     updated based on the state of that Input."""
 
     DEFAULT_CSS = """\
 DropdownChild {
     height: auto;
+    width: auto;
 }
     """
 
     # TODO: Support awaitable and add debounce.
     def __init__(self, linked_input: Input):
         """Construct an Autocomplete. Autocomplete only works if your Screen has a dedicated layer
         called `textual-autocomplete`.
```

### Comparing `textual_autocomplete-2.1.0b0/setup.py` & `textual_autocomplete-3.0.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,141 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: textual-autocomplete
+Version: 3.0.0a0
+Summary: Easily add autocomplete dropdowns to your Textual apps.
+Author: Darren Burns
+Author-email: darrenb900@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: textual (>=0.58.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['textual_autocomplete']
+# textual-autocomplete
 
-package_data = \
-{'': ['*']}
+textual-autocomplete is a Python library for creating dropdown autocompletion menus in
+Textual applications, allowing users to quickly select from a list of suggestions as
+they type. *textual-autocomplete supports **Textual version 0.14.0** and above.*
 
-install_requires = \
-['textual>=0.14.0', 'typing-extensions>=4.5.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'textual-autocomplete',
-    'version': '2.1.0b0',
-    'description': 'Easily add autocomplete dropdowns to your Textual apps.',
-    'long_description': '# textual-autocomplete\n\ntextual-autocomplete is a Python library for creating dropdown autocompletion menus in\nTextual applications, allowing users to quickly select from a list of suggestions as\nthey type. *textual-autocomplete supports **Textual version 0.11.0** and above.*\n\n<img width="554" alt="image" src="https://user-images.githubusercontent.com/5740731/205718538-5599a9db-48a2-49dd-99c3-34d43459b81a.png">\n\n<details>\n<summary>Video example</summary>\n\nhttps://user-images.githubusercontent.com/5740731/205718330-a9364894-9133-40ca-8249-6e3dcc13f456.mov\n\n</details>\n\n> **Warning**\n> Textual still has a major version number of `0`, meaning there are still significant API changes happening which can sometimes impact this project.\n> I\'ll do my best to keep it compatible with the latest version of Textual, but there may be a slight delay between Textual releases and this library working with said release.\n\n## Quickstart\n\nSimply wrap a Textual `Input` widget as follows:\n\n```python\nfrom textual.app import ComposeResult\nfrom textual.widgets import Input\nfrom textual_autocomplete import AutoComplete, Dropdown, DropdownItem\n\ndef compose(self) -> ComposeResult:\n    yield AutoComplete(\n        Input(placeholder="Type to search..."),\n        Dropdown(items=[\n            DropdownItem("Glasgow"),\n            DropdownItem("Edinburgh"),\n            DropdownItem("Aberdeen"),\n            DropdownItem("Dundee"),\n        ]),\n    )\n```\n\nThere are more complete examples [here](./examples).\n\n## Installation\n\n`textual-autocomplete` can be installed from PyPI using your favourite dependency\nmanager.\n\n## Usage\n\n### Wrapping your `Input`\n\nAs shown in the quickstart, you can wrap the Textual builtin `Input` widget with\n`AutoComplete`, and supply a `Dropdown`. \nThe `AutoComplete` manages communication between the `Input` and the `Dropdown`.\n\nThe `Dropdown` is the widget you see on screen, as you type into the input.\n\nThe `DropdownItem`s contain up to 3 columns. All must contain a "main" column, which\nis the central column used in the filtering. They can also optionally contain a left and right metadata\ncolumn.\n\n### Supplying data to `Dropdown`\n\nYou can supply the data for the dropdown via a list or a callback function.\n\n#### Using a list\n\nThe easiest way to use textual-autocomplete is to pass in a list of `DropdownItem`s, \nas shown in the quickstart.\n\n#### Using a callable\n\nInstead of passing a list of `DropdownItems`, you can supply a callback function\nwhich will be called with the current input state. From this function, you should \nreturn the list of `DropdownItems` you wish to be displayed.\n\nSee [here](./examples/custom_meta.py) for a usage example.\n\n### Keyboard control\n\n- Press the Up/Down arrow keys to navigate.\n- Press Enter to select the item in the dropdown and fill it in.\n- Press Tab to fill in the selected item, and move focus.\n- Press Esc to hide the dropdown.\n- Press the Up/Down arrow keys to force the dropdown to appear.\n\n### Styling\n\nThe `Dropdown` itself can be styled using Textual CSS.\n\nFor more fine-grained control over styling, you can target the following CSS classes:\n\n- `.autocomplete--highlight-match`: the highlighted portion of a matching item\n- `.autocomplete--selection-cursor`: the item the selection cursor is on\n- `.autocomplete--left-column`: the left metadata column, if it exists\n- `.autocomplete--right-column`: the right metadata column, if it exists\n\nSince the 3 columns in `DropdownItem` support Rich `Text` objects, they can be styled dynamically.\nThe [custom_meta.py](./examples/custom_meta.py) file is an example of this, showing how the rightmost column is coloured dynamically based on the city population.\n\nThe [examples directory](./examples) contains multiple examples of custom styling.\n\n### Messages\n\nWhen you select an item in the dropdown, an `AutoComplete.Selected` event is emitted.\n\nYou can declare a handler for this event `on_auto_complete_selected(self, event)` to respond\nto an item being selected.\n\nAn item is selected when it\'s highlighted in the dropdown, and you press Enter or Tab.\n\nPressing Enter simply fills the value in the dropdown, whilst Tab fills the value\nand then shifts focus from the input.\n\n## Other notes\n\n- textual-autocomplete will create a new layer at runtime on the `Screen` that the `AutoComplete` is on. The `Dropdown` will be rendered on this layer.\n- The position of the dropdown is currently fixed _below_ the value entered into the `Input`. This means if your `Input` is at the bottom of the screen, it\'s probably not going to be much use for now. I\'m happy to discuss or look at PRs that offer a flag for having it float above.\n- There\'s currently no special handling for when the dropdown meets the right-hand side of the screen.\n- Do not apply `margin` to the `Dropdown`. The position of the dropdown is updated by applying margin to the top/left of it.\n- There\'s currently no debouncing support, but I\'m happy to discuss or look at PRs for this.\n- There are a few known issues/TODOs in the code, which will later be transferred to GitHub.\n- Test coverage is currently non-existent - sorry!\n',
-    'author': 'Darren Burns',
-    'author_email': 'darrenb900@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.8,<4.0.0',
-}
+<img width="554" alt="image" src="https://user-images.githubusercontent.com/5740731/205718538-5599a9db-48a2-49dd-99c3-34d43459b81a.png">
 
+<details>
+<summary>Video example</summary>
+
+https://user-images.githubusercontent.com/5740731/205718330-a9364894-9133-40ca-8249-6e3dcc13f456.mov
+
+</details>
+
+> **Warning**
+> Textual still has a major version number of `0`, meaning there are still significant API changes happening which can sometimes impact this project.
+> I'll do my best to keep it compatible with the latest version of Textual, but there may be a slight delay between Textual releases and this library working with said release.
+
+## Quickstart
+
+Simply wrap a Textual `Input` widget as follows:
+
+```python
+from textual.app import ComposeResult
+from textual.widgets import Input
+from textual_autocomplete import AutoComplete, Dropdown, DropdownItem
+
+def compose(self) -> ComposeResult:
+    yield AutoComplete(
+        Input(placeholder="Type to search..."),
+        Dropdown(items=[
+            DropdownItem("Glasgow"),
+            DropdownItem("Edinburgh"),
+            DropdownItem("Aberdeen"),
+            DropdownItem("Dundee"),
+        ]),
+    )
+```
+
+There are more complete examples [here](./examples).
+
+## Installation
+
+`textual-autocomplete` can be installed from PyPI using your favourite dependency
+manager.
+
+## Usage
+
+### Wrapping your `Input`
+
+As shown in the quickstart, you can wrap the Textual builtin `Input` widget with
+`AutoComplete`, and supply a `Dropdown`. 
+The `AutoComplete` manages communication between the `Input` and the `Dropdown`.
+
+The `Dropdown` is the widget you see on screen, as you type into the input.
+
+The `DropdownItem`s contain up to 3 columns. All must contain a "main" column, which
+is the central column used in the filtering. They can also optionally contain a left and right metadata
+column.
+
+### Supplying data to `Dropdown`
+
+You can supply the data for the dropdown via a list or a callback function.
+
+#### Using a list
+
+The easiest way to use textual-autocomplete is to pass in a list of `DropdownItem`s, 
+as shown in the quickstart.
+
+#### Using a callable
+
+Instead of passing a list of `DropdownItems`, you can supply a callback function
+which will be called with the current input state. From this function, you should 
+return the list of `DropdownItems` you wish to be displayed.
+
+See [here](./examples/custom_meta.py) for a usage example.
+
+### Keyboard control
+
+- Press the Up/Down arrow keys to navigate.
+- Press Enter to select the item in the dropdown and fill it in.
+- Press Tab to fill in the selected item, and move focus.
+- Press Esc to hide the dropdown.
+- Press the Up/Down arrow keys to force the dropdown to appear.
+
+### Styling
+
+The `Dropdown` itself can be styled using Textual CSS.
+
+For more fine-grained control over styling, you can target the following CSS classes:
+
+- `.autocomplete--highlight-match`: the highlighted portion of a matching item
+- `.autocomplete--selection-cursor`: the item the selection cursor is on
+- `.autocomplete--left-column`: the left metadata column, if it exists
+- `.autocomplete--right-column`: the right metadata column, if it exists
+
+Since the 3 columns in `DropdownItem` support Rich `Text` objects, they can be styled dynamically.
+The [custom_meta.py](./examples/custom_meta.py) file is an example of this, showing how the rightmost column is coloured dynamically based on the city population.
+
+The [examples directory](./examples) contains multiple examples of custom styling.
+
+### Messages
+
+When you select an item in the dropdown, an `AutoComplete.Selected` event is emitted.
+
+You can declare a handler for this event `on_auto_complete_selected(self, event)` to respond
+to an item being selected.
+
+An item is selected when it's highlighted in the dropdown, and you press Enter or Tab.
+
+Pressing Enter simply fills the value in the dropdown, whilst Tab fills the value
+and then shifts focus from the input.
+
+## Other notes
+
+- textual-autocomplete will create a new layer at runtime on the `Screen` that the `AutoComplete` is on. The `Dropdown` will be rendered on this layer.
+- The position of the dropdown is currently fixed _below_ the value entered into the `Input`. This means if your `Input` is at the bottom of the screen, it's probably not going to be much use for now. I'm happy to discuss or look at PRs that offer a flag for having it float above.
+- There's currently no special handling for when the dropdown meets the right-hand side of the screen.
+- Do not apply `margin` to the `Dropdown`. The position of the dropdown is updated by applying margin to the top/left of it.
+- There's currently no debouncing support, but I'm happy to discuss or look at PRs for this.
+- There are a few known issues/TODOs in the code, which will later be transferred to GitHub.
+- Test coverage is currently non-existent - sorry!
 
-setup(**setup_kwargs)
```

