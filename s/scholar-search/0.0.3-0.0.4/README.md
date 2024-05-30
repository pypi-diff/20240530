# Comparing `tmp/scholar_search-0.0.3.tar.gz` & `tmp/scholar_search-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scholar_search-0.0.3.tar", last modified: Tue May 14 16:51:12 2024, max compression
+gzip compressed data, was "scholar_search-0.0.4.tar", last modified: Thu May 30 16:22:08 2024, max compression
```

## Comparing `scholar_search-0.0.3.tar` & `scholar_search-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-14 16:51:12.601075 scholar_search-0.0.3/
--rw-r--r--   0 aemiller   (501) staff       (20)     1068 2024-05-14 16:51:06.000000 scholar_search-0.0.3/LICENSE
--rw-r--r--   0 aemiller   (501) staff       (20)      860 2024-05-14 16:51:12.600884 scholar_search-0.0.3/PKG-INFO
--rw-r--r--   0 aemiller   (501) staff       (20)    11694 2024-05-14 16:51:06.000000 scholar_search-0.0.3/README.md
--rw-r--r--   0 aemiller   (501) staff       (20)       81 2024-05-14 16:51:06.000000 scholar_search-0.0.3/pyproject.toml
-drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-14 16:51:12.599882 scholar_search-0.0.3/sch/
--rw-r--r--   0 aemiller   (501) staff       (20)     5065 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/__init__.py
--rw-r--r--   0 aemiller   (501) staff       (20)     2215 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/cli.py
--rw-r--r--   0 aemiller   (501) staff       (20)    27390 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/commands.py
--rw-r--r--   0 aemiller   (501) staff       (20)      123 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/errors.py
--rw-r--r--   0 aemiller   (501) staff       (20)     6921 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/readme.py
--rw-r--r--   0 aemiller   (501) staff       (20)    22322 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/server.py
--rw-r--r--   0 aemiller   (501) staff       (20)     3978 2024-05-14 16:51:06.000000 scholar_search-0.0.3/sch/utils.py
-drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-14 16:51:12.600644 scholar_search-0.0.3/scholar_search.egg-info/
--rw-r--r--   0 aemiller   (501) staff       (20)      860 2024-05-14 16:51:12.000000 scholar_search-0.0.3/scholar_search.egg-info/PKG-INFO
--rw-r--r--   0 aemiller   (501) staff       (20)      369 2024-05-14 16:51:12.000000 scholar_search-0.0.3/scholar_search.egg-info/SOURCES.txt
--rw-r--r--   0 aemiller   (501) staff       (20)        1 2024-05-14 16:51:12.000000 scholar_search-0.0.3/scholar_search.egg-info/dependency_links.txt
--rw-r--r--   0 aemiller   (501) staff       (20)       36 2024-05-14 16:51:12.000000 scholar_search-0.0.3/scholar_search.egg-info/entry_points.txt
--rw-r--r--   0 aemiller   (501) staff       (20)       55 2024-05-14 16:51:12.000000 scholar_search-0.0.3/scholar_search.egg-info/requires.txt
--rw-r--r--   0 aemiller   (501) staff       (20)        4 2024-05-14 16:51:12.000000 scholar_search-0.0.3/scholar_search.egg-info/top_level.txt
--rw-r--r--   0 aemiller   (501) staff       (20)       38 2024-05-14 16:51:12.601114 scholar_search-0.0.3/setup.cfg
--rw-r--r--   0 aemiller   (501) staff       (20)     1097 2024-05-14 16:51:06.000000 scholar_search-0.0.3/setup.py
+drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-30 16:22:08.239743 scholar_search-0.0.4/
+-rw-r--r--   0 aemiller   (501) staff       (20)     1068 2024-05-14 16:51:06.000000 scholar_search-0.0.4/LICENSE
+-rw-r--r--   0 aemiller   (501) staff       (20)      959 2024-05-30 16:22:08.239572 scholar_search-0.0.4/PKG-INFO
+-rw-r--r--   0 aemiller   (501) staff       (20)    14105 2024-05-30 16:19:58.000000 scholar_search-0.0.4/README.md
+-rw-r--r--   0 aemiller   (501) staff       (20)       81 2024-05-14 16:51:06.000000 scholar_search-0.0.4/pyproject.toml
+drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-30 16:22:08.238442 scholar_search-0.0.4/sch/
+-rw-r--r--   0 aemiller   (501) staff       (20)     5071 2024-05-14 17:06:03.000000 scholar_search-0.0.4/sch/__init__.py
+-rw-r--r--   0 aemiller   (501) staff       (20)     2215 2024-05-14 16:51:06.000000 scholar_search-0.0.4/sch/cli.py
+-rw-r--r--   0 aemiller   (501) staff       (20)    29544 2024-05-29 23:51:52.000000 scholar_search-0.0.4/sch/commands.py
+-rw-r--r--   0 aemiller   (501) staff       (20)      123 2024-05-14 16:51:06.000000 scholar_search-0.0.4/sch/errors.py
+-rw-r--r--   0 aemiller   (501) staff       (20)     7145 2024-05-18 01:07:00.000000 scholar_search-0.0.4/sch/readme.py
+-rw-r--r--   0 aemiller   (501) staff       (20)    22322 2024-05-14 16:51:06.000000 scholar_search-0.0.4/sch/server.py
+-rw-r--r--   0 aemiller   (501) staff       (20)     3978 2024-05-14 16:51:06.000000 scholar_search-0.0.4/sch/utils.py
+drwxr-xr-x   0 aemiller   (501) staff       (20)        0 2024-05-30 16:22:08.239224 scholar_search-0.0.4/scholar_search.egg-info/
+-rw-r--r--   0 aemiller   (501) staff       (20)      959 2024-05-30 16:22:08.000000 scholar_search-0.0.4/scholar_search.egg-info/PKG-INFO
+-rw-r--r--   0 aemiller   (501) staff       (20)      369 2024-05-30 16:22:08.000000 scholar_search-0.0.4/scholar_search.egg-info/SOURCES.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)        1 2024-05-30 16:22:08.000000 scholar_search-0.0.4/scholar_search.egg-info/dependency_links.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)       36 2024-05-30 16:22:08.000000 scholar_search-0.0.4/scholar_search.egg-info/entry_points.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)       79 2024-05-30 16:22:08.000000 scholar_search-0.0.4/scholar_search.egg-info/requires.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)        4 2024-05-30 16:22:08.000000 scholar_search-0.0.4/scholar_search.egg-info/top_level.txt
+-rw-r--r--   0 aemiller   (501) staff       (20)       38 2024-05-30 16:22:08.239778 scholar_search-0.0.4/setup.cfg
+-rw-r--r--   0 aemiller   (501) staff       (20)     1129 2024-05-30 14:31:03.000000 scholar_search-0.0.4/setup.py
```

### Comparing `scholar_search-0.0.3/LICENSE` & `scholar_search-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.3/PKG-INFO` & `scholar_search-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scholar-search
-Version: 0.0.3
+Version: 0.0.4
 Summary: a macro search bar
 Home-page: https://github.com/adammillerio/sch
-Download-URL: https://github.com/adammillerio/sch/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/adammillerio/sch/archive/v0.0.4.tar.gz
 Author: Adam Miller
 Author-email: miller@adammiller.io
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,7 +18,10 @@
 License-File: LICENSE
 Requires-Dist: anytree
 Requires-Dist: flask
 Requires-Dist: click
 Requires-Dist: pypandoc
 Provides-Extra: pandoc
 Requires-Dist: pypandoc-binary; extra == "pandoc"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pyre-check; extra == "dev"
```

### Comparing `scholar_search-0.0.3/README.md` & `scholar_search-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 # Clone and run sch against the example codex
 git clone https://github.com/adammillerio/sch.git
 sch run
 ```
 
 And go to http://localhost:5000/sch?s=sch_help for usage info.
 
+The public collection of codexes is available at
+[adammillerio/sch_public](https://github.com/adammillerio/sch_public)
+
 ## Detailed
 
 Scholar can be installed via pip:
 
 ```bash
 # With pandoc
 pip install scholar-search[pandoc]
@@ -332,14 +335,95 @@
         
         if repo:
             return https://github.com/{repo}
         else:
             return https://github.com
 ```
 
+## Command Aliases
+
+Commands can have aliases, which are alternative names that can be used during
+command resolution:
+
+```python
+from sch import codex
+
+@codex.command("help", aliases=["man"])
+def help() -> str:
+    return "/sch?s=sch_help"
+```
+
+```bash
+sch search help sch_help      
+def sch help{man}() -> str:
+        return /sch?s=sch_help
+
+sch search help         
+/sch?s=sch_help
+
+sch search man 
+/sch?s=sch_help
+```
+
+Any command aliases will be displayed in curly braces next to the command name.
+
+## Command Tags
+
+As an alternative method of organization, commands can be tagged on creation or
+during registration:
+
+```python
+from sch import codex
+
+@codex.command("google", tags=["google"])
+def google() -> str:
+    """google search""""
+
+    return "https://google.com"
+
+
+@google.command("drive", tags=["drive"])
+def google_drive() -> str:
+    """google drive"""
+
+    return "https://drive.google.com"
+
+
+@codex.command("youtube", tags=["google", "youtube"])
+def youtube() -> str:
+    """youtube"""
+
+    return "https://youtube.com"
+```
+
+Tags can be used to filter the tree of commands:
+
+```bash
+sch search --tag google sch_tree
+sch - scholar search engine
+|-- google - google search
+|   +-- drive - google drive
++-- youtube - youtube
+
+sch search --tag drive sch_tree
+sch - scholar search engine
++-- google - google search
+   +-- drive - google drive
+
+sch search --tag youtube sch_tree
+sch - scholar search engine
++-- youtube - youtube
+```
+
+Subcommands inherit the tags of their parent command. For example, the `google drive`
+command has both the `drive` tag, and the `google` tag from the parent command.
+
+In the web UI, all tags defined under the current view of commands will be shown
+at the top. Clicking any tag will manually filter to only that tag.
+
 ## Default Command
 
 If a command cannot be resolved during a query, a 404 is returned to the user. Scholar
 can be configured to instead run a default command with all of the provided
 arguments:
 
 ```python
@@ -401,7 +485,35 @@
 The WSGI server itself can then be exposed to the internet via reverse proxy via
 https. Be sure to change the URL scheme when doing this or generated URLs will
 be incorrect:
 
 ```bash
 waitress-serve --port 5000 --url-scheme https --call app:create_app
 ```
+
+# Development
+
+Install in development mode:
+```bash
+pip3 install -e '.[dev]'
+```
+
+## Type Checking
+
+Ensure no type errors are present with [pyre](https://github.com/facebook/pyre-check):
+
+```bash
+pyre check              
+ƛ No type errors found
+```
+
+**Note**: Pyre daemonizes itself on first run for faster subsequent executions. Be
+sure to shut it down with `pyre kill` when finished.
+
+## Formatting
+
+Format code with the [black](https://github.com/psf/black) formatter:
+
+```bash
+black click_tree
+All done! ✨ 🍰 ✨
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scholar_search-0.0.3/sch/__init__.py` & `scholar_search-0.0.4/sch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 
 from sch.commands import bookmark, command, Command, CommandNotFoundError
 from sch.errors import CodexNotFound
 from sch.server import CodexServer
 from sch.utils import format_doc, query_args, escape_args, load_commands
 
 
-@command()
-def default_cmd(*args: str) -> str:
-    """scholar search engine"""
-
-    return "/sch"
-
-
 class Codex(Command):
     """Root Codex
 
     This is the root Node in the Scholar Command tree, and is instantiated to be
     used as a reference point for composing Commands.
 
     Currently all composition is done against a single Codex instance defined
@@ -30,15 +23,20 @@
             run instead of displaying a 404 if no Command can be resolved for
             a given query.
     """
 
     def __init__(self, name: str, default_command: Optional[Command] = None) -> None:
         self._default_command = default_command
 
-        super().__init__(command_func=default_cmd, name=name)
+        def root_cmd(*args: str) -> str:
+            """scholar search engine"""
+
+            return "/sch"
+
+        super().__init__(command_func=root_cmd, name=name)
 
     def get_default_command(self) -> Optional[Command]:
         """Retrieve the default Command.
 
         Returns:
             default_cmd: Optional[Command]. Default command if any.
         """
```

### Comparing `scholar_search-0.0.3/sch/cli.py` & `scholar_search-0.0.4/sch/cli.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.3/sch/commands.py` & `scholar_search-0.0.4/sch/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # inform the user what may be missing.
 # Size of input = 80 chars (terminal) + len(" (?) (>)") = 88 / 2 (readability) = 44
 SCH_HELP = """\
 <form action="/sch"><input type="text" name="s" value="{scope}" autofocus onfocus="this.setSelectionRange(this.value.length,this.value.length);" size="44" spellcheck="false" /></form>
 
 {error_msg}
 
-**def** [{colored_full_scope}](/sch?s={scope_plus}){colored_command_signature}:
+**def** [{colored_full_scope}{colored_alias_names}](/sch?s={scope_plus}){colored_command_signature}:
 ```cyan
     {docstring}
 ```
 """
 
 # Input "REPL": An input box that is autofocused and filled with the current
 # command scope, which will then submit the entry as another command to sch.
@@ -121,43 +121,47 @@
     # HTML mode. Default mode for SCH. Commands return 302 with redirect to link
     # as HTML. All utility commands (tree/help/etc) return HTML via pandoc's
     # markdown -> html converter.
     HTML = "html"
 
 
 def command(
-    name: Optional[str] = None, tags: Optional[Iterable[str]] = None
+    name: Optional[str] = None,
+    tags: Optional[Iterable[str]] = None,
+    aliases: Optional[Iterable[str]] = None,
 ) -> Callable[..., Command]:
     """Create a "generic" command.
 
     This wraps any Scholar compatible function as a Command without attaching
     it to any Codex. This Command can have other Commands registered to it as
     usual in order to compose generic command sets, and can be registered like
     any other Command via add_command.
 
     Args:
         name: Optional[str]. Command Name. If this is not provided at definition,
             it must be provided as an argument to add_command.
         tags: Optional[Iterable[str]]. Tag(s) to apply to this Command.
+        aliases: Optional[Iterable[str]]. Alias name(s) to apply to this Command.
 
     Returns:
         command_decorator: Callable[..., Command]. Decorator for creating a
             Command.
     """
 
     def decorator(func: Callable[..., str]) -> Command:
-        return Command(command_func=func, name=name, tags=tags)
+        return Command(command_func=func, name=name, tags=tags, aliases=aliases)
 
     return decorator
 
 
 def bookmark(
     url: str,
     short_help: Optional[str] = None,
     tags: Optional[Iterable[str]] = None,
+    aliases: Optional[Iterable[str]] = None,
 ) -> Command:
     """Bookmark Command.
 
     A Bookmark Command is just a normal Command that returns a provided URL, with
     no other execution. It also has some custom help formatting.
 
     Bookmarks should be registered using add_bookmark but bookmark can also be
@@ -166,27 +170,27 @@
     All bookmarks have the "bookmark" Command tag.
 
     Args:
         url: str. URL to redirect to for bookmark.
         short_help: Optional[str]. Any additional info to be provided in the
             Command help.
         tags: Optional[Iterable[str]]. Tag(s) to apply to this Command.
-        **kwargs: Any. Forwarded to the @command decorator.
+        aliases: Optional[Iterable[str]]. Alias name(s) to apply to this Command.
 
     Returns:
         bookmark_command: Command.
     """
 
     tag_set = {"bookmark"}
     if tags:
         tag_set.update(tags)
 
     help_str = short_help if short_help else ""
 
-    @command(tags=tag_set)
+    @command(tags=tag_set, aliases=aliases)
     @format_doc(url=url, help_str=help_str)
     def bookmark_command() -> str:
         """{help_str}
 
         return {url}
         """
 
@@ -220,37 +224,44 @@
     Commands can also be tagged with any number of string based tags, which can
     be used for filtering.
 
     Args:
         command_func: Callable[..., str]. Scholar function to wrap.
         name: Optional[str]. Name of this Scholar Command.
         tags: Optional[Iterable[str]]. Tag(s) to apply to this Command.
+        aliases: Optional[Iterable[str]]. Alias name(s) to apply to this Command.
         parent: Optional[Command]. Parent Command, if any.
         children: Optional[Tuple[Command, ...]]. Child (Sub) commands, if any.
     """
 
     # anytree: Switch to space separation instead of /, mostly for UX purposes.
     separator = " "
 
     # anytree: General use Node Resolver for command lookups.
-    resolver: Resolver = Resolver("name")
+    resolver: Resolver = Resolver("name", relax=True)
 
     def __init__(
         self,
         command_func: Callable[..., str],
         name: Optional[str] = None,
         tags: Optional[Iterable[str]] = None,
+        aliases: Optional[Iterable[str]] = None,
         parent: Optional[Command] = None,
         children: Optional[Tuple[Command, ...]] = None,
     ) -> None:
         super().__init__()
 
         self.name = name
         self.command_func = command_func
         self._tags: Set[str] = set(tags) if tags else set()
+        self.aliases: Set[str] = set(aliases) if aliases else set()
+
+        # Mapping of any registered command aliases to the actual child command
+        # name.
+        self.child_aliases: Dict[str, str] = {}
 
         self.parent = parent
         if children:
             self.children: Tuple[Command, ...] = children
 
     @property
     def tags(self) -> Set[str]:
@@ -304,14 +315,21 @@
     def short_help(self) -> str:
         if func_doc := getdoc(self.command_func):
             return func_doc.split("\n")[0]
         else:
             return ""
 
     @property
+    def alias_names(self) -> str:
+        # {foobar}
+        aliases = ",".join(self.aliases)
+
+        return f"{{{aliases}}}" if aliases else ""
+
+    @property
     def scope(self) -> str:
         # gh search
         # Don't include the root Codex in the scope. See full_scope for the
         # same value but inclusive of the Codex.
         return " ".join(node.name for node in self.path[1:])
 
     @property
@@ -338,14 +356,19 @@
 
     @property
     def colored_name(self) -> str:
         # `sch`{.green}
         return f"`{self.name}`{self.color_class}"
 
     @property
+    def colored_alias_names(self) -> str:
+        # `{s}`{.green}
+        return f"`{self.alias_names}`{self.color_class}" if self.alias_names else ""
+
+    @property
     def colored_full_scope(self) -> str:
         """Generate a colored full scope for sch_help.
 
         This uses the color wheel to generate a colored scope of the path leading
         up to this command.
 
         Returns:
@@ -413,78 +436,107 @@
         Returns:
             url: str. URL to redirect to.
         """
 
         return self.command_func(*args)
 
     def get_command(self, name: str) -> Command:
-        try:
-            return self.resolver.get(self, name)
-        except ChildResolverError:
+        if command_name := self.child_aliases.get(name, None):
+            # Name provided is an alias to another command, retrieve it.
+            command = self.resolver.get(self, command_name)
+        else:
+            # Attempt to resolve command with provided name.
+            command = self.resolver.get(self, name)
+
+        if not command:
             raise CommandNotFoundError(f"no command {name} found")
 
+        return command
+
     def add_command(
         self,
         command: Command,
         name: Optional[str] = None,
         tags: Optional[Iterable[str]] = None,
+        aliases: Optional[Iterable[str]] = None,
     ) -> None:
         """Register a Command as a sub-Command.
 
         If a name is provided, it will replace any name defined on the Command
         beforehand.
 
         Args:
             command: Command. Command to register as a sub-Command of this one.
             name: Optional[str]. Name override for Command.
             tags: Optional[Iterable[str]]. Additional tags to apply to Command, if
                 any.
+            aliases: Optional[Iterable[str]]. Alias name(s) to apply to this Command.
 
         Raises:
             ValueError: If a command name was not provided, and the Command has
                 no name.
         """
 
         if name:
             # Name override, set the name on the Command to the expected one. This
             # works alongside composing generic commands with @command()
             command.name = name
         else:
             if not command.name:
                 raise ValueError("command name must be provided")
 
+        if self.resolver.get(self, command.name):
+            raise ValueError(
+                f"command '{self.full_scope}{command.name}' already exists"
+            )
+
         if tags:
             command.tags = set(tags).union(command.tags)
 
         # Inherit all Command tags from the parent.
         command.tags = self.tags.union(command.tags)
 
+        if aliases:
+            command.aliases = set(aliases).union(command.aliases)
+
+        for alias in command.aliases:
+            if existing_alias := self.child_aliases.get(alias, None):
+                raise ValueError(
+                    f"command alias '{self.full_scope}{alias}' to '{existing_alias}' already exists"
+                )
+
+            self.child_aliases[alias] = command.name
+
         # Register the Command.
         command.parent = self
 
     def command(
-        self, name: str, tags: Optional[Iterable[str]] = None
+        self,
+        name: str,
+        tags: Optional[Iterable[str]] = None,
+        aliases: Optional[Iterable[str]] = None,
     ) -> Callable[..., Command]:
         """Create and register a Command to this one.
 
         This wraps any Scholar compatible function as a Command and registers it
         as a sub-Command of this one.
 
         Args:
             name: str. Command name.
             tags: Optional[Iterable[str]]. Tag(s) to apply to this Command.
+            aliases: Optional[Iterable[str]]. Alias name(s) to apply to this Command.
 
         Returns:
             command_decorator: Callable[..., Command]. Decorator for creating and
                 registering the Command.
         """
 
         def decorator(func: Callable[..., str]) -> Command:
             command = Command(name=name, command_func=func, tags=tags)
-            self.add_command(command)
+            self.add_command(command, aliases=aliases)
 
             return command
 
         return decorator
 
     def add_bookmark(
         self,
@@ -528,14 +580,15 @@
         help_str = SCH_HELP.format(
             scope=self.scope,
             scope_plus=self.scope_plus,
             colored_full_scope=self.colored_full_scope,
             docstring=self.docstring,
             command_name=self.name,
             colored_command_signature=self.colored_signature,
+            colored_alias_names=self.colored_alias_names,
             # Don't include code backticks if no error_msg... really just need
             # to switch to jinja...
             error_msg=f"```{{.brcyan}}\n{error_msg}\n```" if error_msg else "",
         ) + SCH_FOOTER.format(sch_title=f"sch ({self.name}?)")
 
         if output_format != OutputFormat.TXT:
             # Back button.
@@ -617,18 +670,18 @@
             # root.
             command_str = node.scope_plus
 
             color_node_name = node.colored_name
             # Add a link to invoking this command on the name itself, using the
             # full path.
             md_node_name = (
-                f"[{node.name}{node.color_class}](/sch?s={command_str})"
+                f"[{node.colored_name}{node.colored_alias_names}](/sch?s={command_str})"
                 if command_str
                 # If it's the root command, just link back to tree.
-                else f"[{node.name}{node.color_class}](/sch?s=sch_tree)"
+                else f"[{node.colored_name}](/sch?s=sch_tree)"
             )
 
             if output_format is not OutputFormat.TXT:
                 # Add a (?) that links to the sch_help for this command.
                 md_help_link = (
                     f" [`?`{node.color_class}](/sch?s={command_str}+sch_help)"
                     if command_str
```

### Comparing `scholar_search-0.0.3/sch/readme.py` & `scholar_search-0.0.4/sch/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 Scholar is open source and is intended to be run locally:
 
 [`sch gh adammillerio/sch`]({full_url}?s=gh+adammillerio/sch) -> [https://github.com/adammillerio/sch](https://github.com/adammillerio/sch)
 
 [`README.md`](https://github.com/adammillerio/sch/blob/main/README.md) provides a guide for getting started. This public instance can still
 be used for demonstration purposes.
 
+The public collection of codexes is also open source:
+
+[`sch gh adammillerio/sch_public`]({full_url}?s=gh+adammillerio/sch_public) -> [https://github.com/adammillerio/sch_public](https://github.com/adammillerio/sch_public)
+
 For instructions on how to set up Scholar in the browser, as well as more general
 information on commands and usage, see below.
 
 ## how to use
 ### chrome(ium) browsers
 Go to `chrome://settings/searchEngines` in the
 address bar (must be typed manually).
@@ -150,15 +154,15 @@
 
 Others are just bookmarks to cool stuff:
 
 [`sch aftermath`]({full_url}?s=aftermath) -> [https://aftermath.site](https://aftermath.site)
 
 ### txt mode
 
-Scholar can be used in the terminal by passing `&smn_txt=true` to any command, which
+Scholar can be used in the terminal by passing `&sch_txt=true` to any command, which
 will enable plain-text only output:
 
 [`curl '{full_url}?s=gh+sch_help&sch_txt=true'`]({full_url}?s=gh+sch_help&sch_txt=true)
 ```sch_docstring
 def gh(repo: Optional[str] = None) -> str:
 
         go to github or a view a repo
```

### Comparing `scholar_search-0.0.3/sch/server.py` & `scholar_search-0.0.4/sch/server.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.3/sch/utils.py` & `scholar_search-0.0.4/sch/utils.py`

 * *Files identical despite different names*

### Comparing `scholar_search-0.0.3/scholar_search.egg-info/PKG-INFO` & `scholar_search-0.0.4/scholar_search.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scholar-search
-Version: 0.0.3
+Version: 0.0.4
 Summary: a macro search bar
 Home-page: https://github.com/adammillerio/sch
-Download-URL: https://github.com/adammillerio/sch/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/adammillerio/sch/archive/v0.0.4.tar.gz
 Author: Adam Miller
 Author-email: miller@adammiller.io
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,7 +18,10 @@
 License-File: LICENSE
 Requires-Dist: anytree
 Requires-Dist: flask
 Requires-Dist: click
 Requires-Dist: pypandoc
 Provides-Extra: pandoc
 Requires-Dist: pypandoc-binary; extra == "pandoc"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pyre-check; extra == "dev"
```

### Comparing `scholar_search-0.0.3/setup.py` & `scholar_search-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 from setuptools import setup, find_packages
 
 setup(
     name="scholar-search",
-    version="0.0.3",
+    version="0.0.4",
     license="MIT",
     description="a macro search bar",
     author="Adam Miller",
     author_email="miller@adammiller.io",
     url="https://github.com/adammillerio/sch",
-    download_url="https://github.com/adammillerio/sch/archive/v0.0.1.tar.gz",
+    download_url="https://github.com/adammillerio/sch/archive/v0.0.4.tar.gz",
     keywords=[],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: End Users/Desktop",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
@@ -25,13 +25,13 @@
     include_package_data=True,
     install_requires=[
         "anytree",
         "flask",
         "click",
         "pypandoc",
     ],
-    extras_require={"pandoc": ["pypandoc-binary"]},
+    extras_require={"pandoc": ["pypandoc-binary"], "dev": ["black", "pyre-check"]},
     entry_points="""
     [console_scripts]
     sch=sch.cli:sch
   """,
 )
```

