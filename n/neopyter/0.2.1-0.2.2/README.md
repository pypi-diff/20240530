# Comparing `tmp/neopyter-0.2.1.tar.gz` & `tmp/neopyter-0.2.2.tar.gz`

## Comparing `neopyter-0.2.1.tar` & `neopyter-0.2.2.tar`

### file list

```diff
@@ -1,103 +1,127 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 neopyter-0.2.1/.commitlintrc.cjs
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 neopyter-0.2.1/.editorconfig
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 neopyter-0.2.1/.eslintignore
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 neopyter-0.2.1/.eslintrc.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 neopyter-0.2.1/.neoconf.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 neopyter-0.2.1/.prettierignore
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 neopyter-0.2.1/.stylua.toml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 neopyter-0.2.1/.yarnrc.yml
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 neopyter-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 neopyter-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 neopyter-0.2.1/Makefile
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 neopyter-0.2.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.1/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neopyter-0.2.1/conftest.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 neopyter-0.2.1/install.json
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 neopyter-0.2.1/jest.config.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 neopyter-0.2.1/jest.polyfills.js
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 neopyter-0.2.1/package.json
--rw-r--r--   0        0        0   345980 2020-02-02 00:00:00.000000 neopyter-0.2.1/pnpm-lock.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 neopyter-0.2.1/pnpm-workspace.yaml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.1/pyrightconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.1/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 neopyter-0.2.1/setup.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 neopyter-0.2.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopyter-0.2.1/tsconfig.test.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 neopyter-0.2.1/.husky/commit-msg
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 neopyter-0.2.1/.husky/pre-commit
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/plugin/cmp_neopyter.lua
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/folds.scm
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/highlights.scm
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/injections.scm
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 neopyter-0.2.1/after/queries/python/textobjects.scm
--rw-r--r--   0        0        0    74924 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/cell_magic.png
--rw-r--r--   0        0        0   799344 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/communication_direct.png
--rw-r--r--   0        0        0  1138980 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/communication_proxy.png
--rw-r--r--   0        0        0    81980 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/completion.png
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/example.ju.py
--rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/line_magic.png
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 neopyter-0.2.1/doc/neopyter.txt
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 neopyter-0.2.1/jupyter-config/server-config/neopyter.json
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter.lua
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/asyncwrap.lua
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/cmp.lua
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/health.lua
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/highlight.lua
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/logger.lua
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/textobjects.lua
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/utils.lua
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/jupyter/init.lua
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/jupyter/jupyterlab.lua
--rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/jupyter/notebook.lua
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/asyncclient.lua
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/baseclient.lua
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/blockclient.lua
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/msgpack.lua
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua/neopyter/rpc/wsserverclient.lua
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 neopyter-0.2.1/lua-tests/neopyter/utils_spec.lua
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/_version.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/handler.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/msgpack_queue.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/tcp_server.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/package.json
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/schemas/neopyter/labplugin.json
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/schemas/neopyter/package.json.orig
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/330.aa97145ed71c9fb187d2.js
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/336.a49647ad642daa70dfb8.js
--rw-r--r--   0        0        0    37319 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/537.62c041ec63a28b9c91aa.js
--rw-r--r--   0        0        0    29596 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/7.8eb9a8e937e5deb3af13.js
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/728.d85cbe66bc2da24c7357.js
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/remoteEntry.dfbe5e3084dd43118cf8.js
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/style.js
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/tests/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 neopyter-0.2.1/neopyter/tests/server/test_handlers.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 neopyter-0.2.1/plugin/neopyter.lua
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 neopyter-0.2.1/schema/labplugin.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 neopyter-0.2.1/scripts/minidoc.lua
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 neopyter-0.2.1/scripts/minimal_init.lua
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/error.ts
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/icons.ts
--rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/index.ts
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/msgpackRpcProtocol.ts
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/rpcServer.ts
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/settings.ts
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/statusidepanel.ts
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/svg.d.ts
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/__tests__/neojupy.spec.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/dispatcher/basic.ts
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/dispatcher/docmanager.ts
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/base.ts
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/index.ts
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/reverseHttpTransport.ts
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 neopyter-0.2.1/src/transport/websocketTransport.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/index.js
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 neopyter-0.2.1/style/icons/statuspage.svg
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 neopyter-0.2.1/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 neopyter-0.2.1/LICENSE
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 neopyter-0.2.1/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 neopyter-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 neopyter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 neopyter-0.2.2/.commitlintrc.cjs
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 neopyter-0.2.2/.editorconfig
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 neopyter-0.2.2/.eslintignore
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 neopyter-0.2.2/.eslintrc.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 neopyter-0.2.2/.neoconf.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 neopyter-0.2.2/.prettierignore
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 neopyter-0.2.2/.stylua.toml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 neopyter-0.2.2/.yarnrc.yml
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 neopyter-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 neopyter-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 neopyter-0.2.2/Makefile
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 neopyter-0.2.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.2/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 neopyter-0.2.2/conftest.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 neopyter-0.2.2/install.json
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 neopyter-0.2.2/jest.config.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 neopyter-0.2.2/jest.polyfills.js
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 neopyter-0.2.2/package.json
+-rw-r--r--   0        0        0   382752 2020-02-02 00:00:00.000000 neopyter-0.2.2/pnpm-lock.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 neopyter-0.2.2/pnpm-workspace.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 neopyter-0.2.2/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.2/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 neopyter-0.2.2/setup.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 neopyter-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 neopyter-0.2.2/tsconfig.test.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 neopyter-0.2.2/.husky/commit-msg
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 neopyter-0.2.2/.husky/pre-commit
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 neopyter-0.2.2/after/plugin/cmp_neopyter.lua
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.2/after/queries/python/folds.scm
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 neopyter-0.2.2/after/queries/python/highlights.scm
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 neopyter-0.2.2/after/queries/python/injections.scm
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 neopyter-0.2.2/after/queries/python/textobjects.scm
+-rw-r--r--   0        0        0    74924 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/cell_magic.png
+-rw-r--r--   0        0        0   799344 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/communication_direct.png
+-rw-r--r--   0        0        0  1138980 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/communication_proxy.png
+-rw-r--r--   0        0        0    81980 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/completion.png
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/example.ju.py
+-rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/line_magic.png
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/neopyter.txt
+-rw-r--r--   0        0        0    60285 2020-02-02 00:00:00.000000 neopyter-0.2.2/doc/sidepanel.png
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 neopyter-0.2.2/jupyter-config/server-config/neopyter.json
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter.lua
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/asyncwrap.lua
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/cmp.lua
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/health.lua
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/highlight.lua
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/logger.lua
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/textobjects.lua
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/utils.lua
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/jupyter/init.lua
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/jupyter/jupyterlab.lua
+-rw-r--r--   0        0        0     9926 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/jupyter/notebook.lua
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/rpc/asyncclient.lua
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/rpc/baseclient.lua
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/rpc/blockclient.lua
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/rpc/msgpack.lua
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua/neopyter/rpc/wsserverclient.lua
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 neopyter-0.2.2/lua-tests/neopyter/utils_spec.lua
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/_version.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/handler.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/msgpack_queue.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/tcp_server.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/package.json
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/schemas/neopyter/labplugin.json
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/schemas/neopyter/package.json.orig
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/221.a3da87512f425651ce5e.js
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/260.7c1e16965abe1ac060cd.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/260.7c1e16965abe1ac060cd.js.LICENSE.txt
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/275.507ccaf7647ff3161123.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/275.507ccaf7647ff3161123.js.LICENSE.txt
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/330.502c5d98d7f9486eb06c.js
+-rw-r--r--   0        0        0    10342 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/404.ed688261aeaa50ea3c80.js
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/51.8adf337e32b058b38bce.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/51.8adf337e32b058b38bce.js.LICENSE.txt
+-rw-r--r--   0        0        0    37320 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/537.802da0d3fc85242e2b5b.js
+-rw-r--r--   0        0        0   140709 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/63.d371004f9c806432884a.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/63.d371004f9c806432884a.js.LICENSE.txt
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/656.eb451b691f1f57dfbddd.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/656.eb451b691f1f57dfbddd.js.LICENSE.txt
+-rw-r--r--   0        0        0    29599 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/7.ff6c4288ceb2d2054177.js
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/728.4d0c9af16f4fa2e12590.js
+-rw-r--r--   0        0        0    63185 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/755.d419d5b684a8edd7d772.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/755.d419d5b684a8edd7d772.js.LICENSE.txt
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/824.1e36c256cc59d1870d6f.js
+-rw-r--r--   0        0        0  1428194 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/833.f82d7adfbd3f63711964.js
+-rw-r--r--   0        0        0    36299 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/833.f82d7adfbd3f63711964.js.LICENSE.txt
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/879.291a46a4de08db938f7f.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/879.291a46a4de08db938f7f.js.LICENSE.txt
+-rw-r--r--   0        0        0    17889 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/916.b27c9b34601e3b28e1a8.js
+-rw-r--r--   0        0        0    52798 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/930.f504db5ecec088dc3aef.js
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/930.f504db5ecec088dc3aef.js.LICENSE.txt
+-rw-r--r--   0        0        0    68323 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/97.96358f068504ce9a8659.js
+-rw-r--r--   0        0        0    10689 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/remoteEntry.998806a05dd33ef36680.js
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/style.js
+-rw-r--r--   0        0        0   171473 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/tests/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 neopyter-0.2.2/neopyter/tests/server/test_handlers.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 neopyter-0.2.2/plugin/neopyter.lua
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 neopyter-0.2.2/schema/labplugin.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 neopyter-0.2.2/scripts/minidoc.lua
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 neopyter-0.2.2/scripts/minimal_init.lua
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/error.ts
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/icons.ts
+-rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/index.ts
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/msgpackRpcProtocol.ts
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/rpcServer.ts
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/statusidepanel.tsx
+-rwxr-xr-x   0        0        0     3879 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/store.ts
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/svg.d.ts
+-rwxr-xr-x   0        0        0     3419 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/utilitytype.ts
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/__tests__/neojupy.spec.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/dispatcher/basic.ts
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/dispatcher/docmanager.ts
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/transport/base.ts
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/transport/index.ts
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/transport/reverseHttpTransport.ts
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 neopyter-0.2.2/src/transport/websocketTransport.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 neopyter-0.2.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 neopyter-0.2.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 neopyter-0.2.2/style/index.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 neopyter-0.2.2/style/icons/statuspage.svg
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 neopyter-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 neopyter-0.2.2/LICENSE
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 neopyter-0.2.2/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 neopyter-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    12286 2020-02-02 00:00:00.000000 neopyter-0.2.2/PKG-INFO
```

### Comparing `neopyter-0.2.1/.eslintrc.json` & `neopyter-0.2.2/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/CHANGELOG.md` & `neopyter-0.2.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/CONTRIBUTING.md` & `neopyter-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/RELEASE.md` & `neopyter-0.2.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/jest.config.js` & `neopyter-0.2.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/package.json` & `neopyter-0.2.2/neopyter/labextension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9627926421404682%*

 * *Differences: {"'dependencies'": "{'@rjsf/antd': '^5.18.2', '@rjsf/core': '^5.18.2', '@rjsf/utils': '^5.18.2', "*

 * *                   "'@rjsf/validator-ajv8': '^5.18.2', 'antd': '^5.16.2', 'zustand': '^4.5.2'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.998806a05dd33ef36680.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -9,15 +9,21 @@
     "dependencies": {
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.2.5",
         "@jupyterlab/logconsole": "^4.1.5",
         "@jupyterlab/notebook": "^4.1.5",
         "@lumino/widgets": "^2.3.1",
         "@msgpack/msgpack": "3.0.0-beta2",
-        "remeda": "^1.55.0"
+        "@rjsf/antd": "^5.18.2",
+        "@rjsf/core": "^5.18.2",
+        "@rjsf/utils": "^5.18.2",
+        "@rjsf/validator-ajv8": "^5.18.2",
+        "antd": "^5.16.2",
+        "remeda": "^1.55.0",
+        "zustand": "^4.5.2"
     },
     "description": "A JupyterLab extension. Integrate JupyterLab and Neovim",
     "devDependencies": {
         "@commitlint/cli": "^18.6.1",
         "@commitlint/config-conventional": "^18.6.3",
         "@jupyterlab/builder": "^4.1.5",
         "@jupyterlab/completer": "^4.1.5",
@@ -54,14 +60,19 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/SUSTech-data/neopyter",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.998806a05dd33ef36680.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "neopyter/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -135,12 +146,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1",
+    "version": "0.2.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `neopyter-0.2.1/pnpm-lock.yaml` & `neopyter-0.2.2/pnpm-lock.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,35 @@
         version: 4.1.5
       '@lumino/widgets':
         specifier: ^2.3.1
         version: 2.3.1
       '@msgpack/msgpack':
         specifier: 3.0.0-beta2
         version: 3.0.0-beta2
+      '@rjsf/antd':
+        specifier: ^5.18.2
+        version: 5.18.2(@ant-design/icons@5.3.6)(@rjsf/core@5.18.2)(@rjsf/utils@5.18.2)(antd@5.16.2)(dayjs@1.11.10)(react-dom@18.2.0)(react@18.2.0)
+      '@rjsf/core':
+        specifier: ^5.18.2
+        version: 5.18.2(@rjsf/utils@5.18.2)(react@18.2.0)
+      '@rjsf/utils':
+        specifier: ^5.18.2
+        version: 5.18.2(react@18.2.0)
+      '@rjsf/validator-ajv8':
+        specifier: ^5.18.2
+        version: 5.18.2(@rjsf/utils@5.18.2)
+      antd:
+        specifier: ^5.16.2
+        version: 5.16.2(react-dom@18.2.0)(react@18.2.0)
       remeda:
         specifier: ^1.55.0
         version: 1.55.0
+      zustand:
+        specifier: ^4.5.2
+        version: 4.5.2(react@18.2.0)
     devDependencies:
       '@commitlint/cli':
         specifier: ^18.6.1
         version: 18.6.1(@types/node@20.11.30)(typescript@5.0.4)
       '@commitlint/config-conventional':
         specifier: ^18.6.3
         version: 18.6.3
@@ -150,14 +168,70 @@
     resolution: {integrity: sha512-30iZtAPgz+LTIYoeivqYo853f02jBYSd5uGnGpkFV0M3xOt9aN73erkgYAmZU43x4VfqcnLxW9Kpg3R5LC4YYw==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/gen-mapping': 0.3.5
       '@jridgewell/trace-mapping': 0.3.25
     dev: true
 
+  /@ant-design/colors@7.0.2:
+    resolution: {integrity: sha512-7KJkhTiPiLHSu+LmMJnehfJ6242OCxSlR3xHVBecYxnMW8MS/878NXct1GqYARyL59fyeFdKRxXTfvR9SnDgJg==}
+    dependencies:
+      '@ctrl/tinycolor': 3.6.1
+    dev: false
+
+  /@ant-design/cssinjs@1.19.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-hgQ3wiys3X0sqDKWkqCJ6EYdF79i9JCvtavmIGwuuPUKmoJXV8Ff0sY+yQQSxk2dRmMyam/bYKo/Bwor45hnZw==}
+    peerDependencies:
+      react: '>=16.0.0'
+      react-dom: '>=16.0.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@emotion/hash': 0.8.0
+      '@emotion/unitless': 0.7.5
+      classnames: 2.5.1
+      csstype: 3.1.3
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+      stylis: 4.3.1
+    dev: false
+
+  /@ant-design/icons-svg@4.4.2:
+    resolution: {integrity: sha512-vHbT+zJEVzllwP+CM+ul7reTEfBR0vgxFe7+lREAsAA7YGsYpboiq2sQNeQeRvh09GfQgs/GyFEvZpJ9cLXpXA==}
+    dev: false
+
+  /@ant-design/icons@5.3.6(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-JeWsgNjvkTTC73YDPgWOgdScRku/iHN9JU0qk39OSEmJSCiRghQMLlxGTCY5ovbRRoXjxHXnUKgQEgBDnQfKmA==}
+    engines: {node: '>=8'}
+    peerDependencies:
+      react: '>=16.0.0'
+      react-dom: '>=16.0.0'
+    dependencies:
+      '@ant-design/colors': 7.0.2
+      '@ant-design/icons-svg': 4.4.2
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@ant-design/react-slick@1.1.2(react@18.2.0):
+    resolution: {integrity: sha512-EzlvzE6xQUBrZuuhSAFTdsr4P2bBBHGZwKFemEfq8gIGyIQCxalYfZW/T2ORbtQx5rU69o+WycP3exY/7T1hGA==}
+    peerDependencies:
+      react: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      json2mq: 0.2.0
+      react: 18.2.0
+      resize-observer-polyfill: 1.5.1
+      throttle-debounce: 5.0.0
+    dev: false
+
   /@babel/code-frame@7.24.2:
     resolution: {integrity: sha512-y5+tLQyV8pg3fsiln67BVLD1P13Eg4lh5RW9mF0zUuvLrv9uIQ4MCL+CRT+FTsBlBjcIan6PGsLcBN0m3ClUyQ==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/highlight': 7.24.2
       picocolors: 1.0.0
     dev: true
@@ -1308,14 +1382,21 @@
   /@babel/runtime@7.24.1:
     resolution: {integrity: sha512-+BIznRzyqBf+2wCTxcKE3wDjfGeCoVE61KSHGpkzqrLi8qxqFwBeUFyId2cxkTmm55fzDGnm0+yCxaxygrLUnQ==}
     engines: {node: '>=6.9.0'}
     dependencies:
       regenerator-runtime: 0.14.1
     dev: true
 
+  /@babel/runtime@7.24.4:
+    resolution: {integrity: sha512-dkxf7+hn8mFBwKjs9bvBlArzLVxVbS8usaPUDd5p2a9JCL9tB8OaOVN1isD4+Xyk4ns89/xeOmbQvgdK7IIVdA==}
+    engines: {node: '>=6.9.0'}
+    dependencies:
+      regenerator-runtime: 0.14.1
+    dev: false
+
   /@babel/template@7.24.0:
     resolution: {integrity: sha512-Bkf2q8lMB0AFpX0NFEqSbx1OkTHf0f+0j82mkw+ZpzBnkk7e9Ql0891vlfgi+kHwOk8tQjiQHpqh4LaSa0fKEA==}
     engines: {node: '>=6.9.0'}
     dependencies:
       '@babel/code-frame': 7.24.2
       '@babel/parser': 7.24.1
       '@babel/types': 7.24.0
@@ -1727,19 +1808,32 @@
     engines: {node: ^14 || ^16 || >=18}
     peerDependencies:
       postcss-selector-parser: ^6.0.13
     dependencies:
       postcss-selector-parser: 6.0.16
     dev: true
 
+  /@ctrl/tinycolor@3.6.1:
+    resolution: {integrity: sha512-SITSV6aIXsuVNV3f3O0f2n/cgyEDWoSqtZMYiAmcsYHydcKrOz3gUxB/iXd/Qf08+IZX4KpgNbvUdMBmWz+kcA==}
+    engines: {node: '>=10'}
+    dev: false
+
   /@discoveryjs/json-ext@0.5.7:
     resolution: {integrity: sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==}
     engines: {node: '>=10.0.0'}
     dev: true
 
+  /@emotion/hash@0.8.0:
+    resolution: {integrity: sha512-kBJtf7PH6aWwZ6fka3zQ0p6SBYzx4fl1LoZXE2RrnYST9Xljm7WfKJrU4g/Xr3Beg72MLrp1AWNUmuYJTL7Cow==}
+    dev: false
+
+  /@emotion/unitless@0.7.5:
+    resolution: {integrity: sha512-OWORNpfjMsSSUBVrRBVGECkhWcULOAJz9ZW8uK9qgxD+87M7jHRcvh/A96XXNhXTLmKcoYSQtBEX7lHMO7YRwg==}
+    dev: false
+
   /@eslint-community/eslint-utils@4.4.0(eslint@8.57.0):
     resolution: {integrity: sha512-1/sA4dwrzBAyeUoQ6oxahHKmrZvsnLCg4RfxW3ZFGGmQkSNQPFNLV9CUEFQP1x9EYXHTo5p6xdhZM1Ne9p/AfA==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     peerDependencies:
       eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
     dependencies:
       eslint: 8.57.0
@@ -3167,14 +3261,133 @@
     resolution: {integrity: sha512-EaaawMTOeEItCRvfmkI9v6rBkF1svM8wjl/YPRrg2N2Wmp+4qJYkWtJsbew1szfKKDm6fPLy4YAanBhIlf9dWw==}
     engines: {node: '>=16'}
     hasBin: true
     dependencies:
       playwright: 1.40.1
     dev: true
 
+  /@rc-component/color-picker@1.5.3(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-+tGGH3nLmYXTalVe0L8hSZNs73VTP5ueSHwUlDC77KKRaN7G4DS4wcpG5DTDzdcV/Yas+rzA6UGgIyzd8fS4cw==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@ctrl/tinycolor': 3.6.1
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@rc-component/context@1.4.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-kFcNxg9oLRMoL3qki0OMxK+7g5mypjgaaJp/pkOis/6rVxma9nJBF/8kCIuTYHUQNr0ii7MxqE33wirPZLJQ2w==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@rc-component/mini-decimal@1.1.0:
+    resolution: {integrity: sha512-jS4E7T9Li2GuYwI6PyiVXmxTiM6b07rlD9Ge8uGZSCz3WlzcG5ZK7g5bbuKNeZ9pgUuPK/5guV781ujdVpm4HQ==}
+    engines: {node: '>=8.x'}
+    dependencies:
+      '@babel/runtime': 7.24.4
+    dev: false
+
+  /@rc-component/mutate-observer@1.1.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-QjrOsDXQusNwGZPf4/qRQasg7UFEj06XiCJ8iuiq/Io7CrHrgVi6Uuetw60WAMG1799v+aM8kyc+1L/GBbHSlw==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@rc-component/portal@1.1.2(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-6f813C0IsasTZms08kfA8kPAGxbbkYToa8ALaiDIGGECU4i9hj8Plgbx0sNJDrey3EtHO30hmdaxtT0138xZcg==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@rc-component/tour@1.14.2(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-A75DZ8LVvahBIvxooj3Gvf2sxe+CGOkmzPNX7ek0i0AJHyKZ1HXe5ieIGo3m0FMdZfVOlbCJ952Duq8VKAHk6g==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/portal': 1.1.2(react-dom@18.2.0)(react@18.2.0)
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@rc-component/trigger@2.1.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-UjHkedkgtEcgQu87w1VuWug1idoDJV7VUt0swxHXRcmei2uu1AuUzGBPEUlmOmXGJ+YtTgZfVLi7kuAUKoZTMA==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/portal': 1.1.2(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /@rjsf/antd@5.18.2(@ant-design/icons@5.3.6)(@rjsf/core@5.18.2)(@rjsf/utils@5.18.2)(antd@5.16.2)(dayjs@1.11.10)(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-JoICg55EHEx02WekH+NvywOBa22SiLASxCn+pvWcQm16bfktexn76LRD5mDGjSoi8TNocCTBWHYZja6nhMwEfA==}
+    engines: {node: '>=14'}
+    peerDependencies:
+      '@ant-design/icons': ^4.0.0 || ^5.0.0
+      '@rjsf/core': ^5.18.x
+      '@rjsf/utils': ^5.18.x
+      antd: ^4.24.0 || ^5.8.5
+      dayjs: ^1.8.0
+      react: ^16.14.0 || >=17
+    dependencies:
+      '@ant-design/icons': 5.3.6(react-dom@18.2.0)(react@18.2.0)
+      '@rjsf/core': 5.18.2(@rjsf/utils@5.18.2)(react@18.2.0)
+      '@rjsf/utils': 5.18.2(react@18.2.0)
+      antd: 5.16.2(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      dayjs: 1.11.10
+      lodash: 4.17.21
+      lodash-es: 4.17.21
+      rc-picker: 2.7.6(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+    transitivePeerDependencies:
+      - react-dom
+    dev: false
+
   /@rjsf/core@5.17.1(@rjsf/utils@5.17.1)(react@18.2.0):
     resolution: {integrity: sha512-COZSuumwHskWN8Pz3RxdxvuQUP6M/qBMXAkIi+TSWLFLaF6SUugpLiceMT1jGemDCr7fOSTiPxjkToSsgpvueQ==}
     engines: {node: '>=14'}
     peerDependencies:
       '@rjsf/utils': ^5.16.x
       react: ^16.14.0 || >=17
     dependencies:
@@ -3182,27 +3395,70 @@
       lodash: 4.17.21
       lodash-es: 4.17.21
       markdown-to-jsx: 7.4.3(react@18.2.0)
       nanoid: 3.3.7
       prop-types: 15.8.1
       react: 18.2.0
 
+  /@rjsf/core@5.18.2(@rjsf/utils@5.18.2)(react@18.2.0):
+    resolution: {integrity: sha512-dqS8E70DJSnTpJ8tdQi4flTffJ3fr/G1Jro7Bhx/eKiB2UbYII1tR536HfZqwe8p1NvJ26DViJclOAghHPmJog==}
+    engines: {node: '>=14'}
+    peerDependencies:
+      '@rjsf/utils': ^5.18.x
+      react: ^16.14.0 || >=17
+    dependencies:
+      '@rjsf/utils': 5.18.2(react@18.2.0)
+      lodash: 4.17.21
+      lodash-es: 4.17.21
+      markdown-to-jsx: 7.4.3(react@18.2.0)
+      nanoid: 3.3.7
+      prop-types: 15.8.1
+      react: 18.2.0
+    dev: false
+
   /@rjsf/utils@5.17.1(react@18.2.0):
     resolution: {integrity: sha512-q1Igz/cuM2hi+jiXFkoaXqdRTUFB+a0jfVKNmZlHmvPmfYeeJfcfyOTzO8dQ41fHNHUFb15ryxa/TblDQimwkA==}
     engines: {node: '>=14'}
     peerDependencies:
       react: ^16.14.0 || >=17
     dependencies:
       json-schema-merge-allof: 0.8.1
       jsonpointer: 5.0.1
       lodash: 4.17.21
       lodash-es: 4.17.21
       react: 18.2.0
       react-is: 18.2.0
 
+  /@rjsf/utils@5.18.2(react@18.2.0):
+    resolution: {integrity: sha512-iDqwBTispZ7mAgwBuHIM0emK+Ft2xRgKD9TzB68VEUhr2hqlDRpwtH6/AgAWUKmJl4kUj3cRKVqqhIvamGLpXw==}
+    engines: {node: '>=14'}
+    peerDependencies:
+      react: ^16.14.0 || >=17
+    dependencies:
+      json-schema-merge-allof: 0.8.1
+      jsonpointer: 5.0.1
+      lodash: 4.17.21
+      lodash-es: 4.17.21
+      react: 18.2.0
+      react-is: 18.2.0
+    dev: false
+
+  /@rjsf/validator-ajv8@5.18.2(@rjsf/utils@5.18.2):
+    resolution: {integrity: sha512-TG2PP6wp1DSLBEF+v49fgGj3VCzxKewxvQvfycEZUkEvmWggca4vYzJdSm0RtMxyOGT80i54oKGnyDv13wxJkg==}
+    engines: {node: '>=14'}
+    peerDependencies:
+      '@rjsf/utils': ^5.18.x
+    dependencies:
+      '@rjsf/utils': 5.18.2(react@18.2.0)
+      ajv: 8.12.0
+      ajv-formats: 2.1.1(ajv@8.12.0)
+      lodash: 4.17.21
+      lodash-es: 4.17.21
+    dev: false
+
   /@sinclair/typebox@0.27.8:
     resolution: {integrity: sha512-+Fj43pSMwJs4KRrH/938Uf+uAELIgVBmQzg/q1YG10djyfA3TnrU8N8XzqCh/okZdszqBQTZf96idMfE5lnwTA==}
     dev: true
 
   /@sinonjs/commons@3.0.1:
     resolution: {integrity: sha512-K3mCHKQ9sVh8o1C9cxkwxaOmXoAMlDxC1mYyHrjqOWEcBjYr76t96zL2zlj5dUGZ3HSw240X1qgH3Mjf1yJWpQ==}
     dependencies:
@@ -4126,15 +4382,14 @@
     peerDependencies:
       ajv: ^8.0.0
     peerDependenciesMeta:
       ajv:
         optional: true
     dependencies:
       ajv: 8.12.0
-    dev: true
 
   /ajv-keywords@3.5.2(ajv@6.12.6):
     resolution: {integrity: sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==}
     peerDependencies:
       ajv: ^6.9.1
     dependencies:
       ajv: 6.12.6
@@ -4203,14 +4458,76 @@
     dev: true
 
   /ansi-styles@6.2.1:
     resolution: {integrity: sha512-bN798gFfQX+viw3R7yrGWRqnrN2oRkEkUjjl4JNn4E8GxxbjtG3FbrEIIY3l8/hrwUwIeCZvi4QuOTP4MErVug==}
     engines: {node: '>=12'}
     dev: true
 
+  /antd@5.16.2(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-46BC1IaCRzkdcTAs1TuIZ1D56JrIRP5yWGrlfV+kGjro1c2dVaQP7yGXA2/m29uF41TqptxOYl36opY5ydN++A==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@ant-design/colors': 7.0.2
+      '@ant-design/cssinjs': 1.19.1(react-dom@18.2.0)(react@18.2.0)
+      '@ant-design/icons': 5.3.6(react-dom@18.2.0)(react@18.2.0)
+      '@ant-design/react-slick': 1.1.2(react@18.2.0)
+      '@babel/runtime': 7.24.4
+      '@ctrl/tinycolor': 3.6.1
+      '@rc-component/color-picker': 1.5.3(react-dom@18.2.0)(react@18.2.0)
+      '@rc-component/mutate-observer': 1.1.0(react-dom@18.2.0)(react@18.2.0)
+      '@rc-component/tour': 1.14.2(react-dom@18.2.0)(react@18.2.0)
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      copy-to-clipboard: 3.3.3
+      dayjs: 1.11.10
+      qrcode.react: 3.1.0(react@18.2.0)
+      rc-cascader: 3.24.1(react-dom@18.2.0)(react@18.2.0)
+      rc-checkbox: 3.2.0(react-dom@18.2.0)(react@18.2.0)
+      rc-collapse: 3.7.3(react-dom@18.2.0)(react@18.2.0)
+      rc-dialog: 9.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-drawer: 7.1.0(react-dom@18.2.0)(react@18.2.0)
+      rc-dropdown: 4.2.0(react-dom@18.2.0)(react@18.2.0)
+      rc-field-form: 1.44.0(react-dom@18.2.0)(react@18.2.0)
+      rc-image: 7.6.0(react-dom@18.2.0)(react@18.2.0)
+      rc-input: 1.4.5(react-dom@18.2.0)(react@18.2.0)
+      rc-input-number: 9.0.0(react-dom@18.2.0)(react@18.2.0)
+      rc-mentions: 2.11.1(react-dom@18.2.0)(react@18.2.0)
+      rc-menu: 9.13.0(react-dom@18.2.0)(react@18.2.0)
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-notification: 5.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-pagination: 4.0.4(react-dom@18.2.0)(react@18.2.0)
+      rc-picker: 4.3.2(dayjs@1.11.10)(react-dom@18.2.0)(react@18.2.0)
+      rc-progress: 4.0.0(react-dom@18.2.0)(react@18.2.0)
+      rc-rate: 2.12.0(react-dom@18.2.0)(react@18.2.0)
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-segmented: 2.3.0(react-dom@18.2.0)(react@18.2.0)
+      rc-select: 14.13.1(react-dom@18.2.0)(react@18.2.0)
+      rc-slider: 10.5.0(react-dom@18.2.0)(react@18.2.0)
+      rc-steps: 6.0.1(react-dom@18.2.0)(react@18.2.0)
+      rc-switch: 4.1.0(react-dom@18.2.0)(react@18.2.0)
+      rc-table: 7.45.4(react-dom@18.2.0)(react@18.2.0)
+      rc-tabs: 14.1.1(react-dom@18.2.0)(react@18.2.0)
+      rc-textarea: 1.6.3(react-dom@18.2.0)(react@18.2.0)
+      rc-tooltip: 6.2.0(react-dom@18.2.0)(react@18.2.0)
+      rc-tree: 5.8.5(react-dom@18.2.0)(react@18.2.0)
+      rc-tree-select: 5.19.0(react-dom@18.2.0)(react@18.2.0)
+      rc-upload: 4.5.2(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+      scroll-into-view-if-needed: 3.1.0
+      throttle-debounce: 5.0.0
+    transitivePeerDependencies:
+      - date-fns
+      - luxon
+      - moment
+    dev: false
+
   /anymatch@3.1.3:
     resolution: {integrity: sha512-KMReFUr0B4t+D+OBkjR3KYqvocp2XaSzO55UcB6mgQMd3KbcE+mWTyvVV7D/zsdEbNnV6acZUutkiHQXvTr1Rw==}
     engines: {node: '>= 8'}
     dependencies:
       normalize-path: 3.0.0
       picomatch: 2.3.1
     dev: true
@@ -4233,14 +4550,18 @@
       is-array-buffer: 3.0.4
     dev: true
 
   /array-ify@1.0.0:
     resolution: {integrity: sha1-nlKHYrSpBmrRY6aWKjZEGOlibs4=}
     dev: true
 
+  /array-tree-filter@2.1.0:
+    resolution: {integrity: sha512-4ROwICNlNw/Hqa9v+rk5h22KjmzB1JGTMVKP2AKJBOCgb0yL0ASf0+YvCcLNNwquOHNX48jkeZIJ3a+oOQqKcw==}
+    dev: false
+
   /array-union@2.1.0:
     resolution: {integrity: sha512-HGyxoOTYUyCM6stUe6EJgnd4EoewAI7zMdfqO+kGjnlZmBDz/cR5pf8r/cR4Wq60sL/p0IkcjUEEPwS3GFrIyw==}
     engines: {node: '>=8'}
     dev: true
 
   /arraybuffer.prototype.slice@1.0.3:
     resolution: {integrity: sha512-bMxMKAjg13EBSVscxTaYA4mRc5t1UAXa2kXiGTNfZ079HIWXEkKmkgFrh/nJqamaLSrXO5H4WFFkPEaLJWbs3A==}
@@ -4262,14 +4583,18 @@
     dev: true
 
   /astral-regex@2.0.0:
     resolution: {integrity: sha512-Z7tMw1ytTXt5jqMcOP+OQteU1VuNK9Y02uuJtKQ1Sv69jXQKKg5cibLwGJow8yzZP+eAc18EmLGPal0bp36rvQ==}
     engines: {node: '>=8'}
     dev: true
 
+  /async-validator@4.2.5:
+    resolution: {integrity: sha512-7HhHjtERjqlNbZtqNqy2rckN/SpOOlmDliet+lP7k+eKZEjPk3DgyeU9lIXLdeLz0uBbbVp+9Qdow9wJWgwwfg==}
+    dev: false
+
   /asynckit@0.4.0:
     resolution: {integrity: sha1-x57Zf380y48robyXkLzDZkdLS3k=}
     dev: true
 
   /available-typed-arrays@1.0.7:
     resolution: {integrity: sha512-wvUjBtSGN7+7SjNpq/9M2Tg350UZD3q62IFZLbRAR1bSMlCo1ZaeW+BJ+D090e4hIIZLBcTDWe4Mh4jvUDajzQ==}
     engines: {node: '>= 0.4'}
@@ -4530,14 +4855,18 @@
     engines: {node: '>=8'}
     dev: true
 
   /cjs-module-lexer@1.2.3:
     resolution: {integrity: sha512-0TNiGstbQmCFwt4akjjBg5pLRTSyj/PkWQ1ZoO2zntmg9yLqSRxwEa4iCfQLGjqhiqBfOJa7W/E8wfGrTDmlZQ==}
     dev: true
 
+  /classnames@2.5.1:
+    resolution: {integrity: sha512-saHYOzhIQs6wy2sVxTM6bUDsQO4F50V9RQ22qBpEdCW+I+/Wmke2HOl6lS6dTpdxVhb88/I6+Hs+438c3lfUow==}
+    dev: false
+
   /cliui@8.0.1:
     resolution: {integrity: sha512-BSeNnyus75C4//NQ9gQt1/csTXyo/8Sb+afLAkzAptFuMsod9HFokGNudZpi/oQV73hnVK+sR+5PVRMd+Dr7YQ==}
     engines: {node: '>=12'}
     dependencies:
       string-width: 4.2.3
       strip-ansi: 6.0.1
       wrap-ansi: 7.0.0
@@ -4634,14 +4963,18 @@
     resolution: {integrity: sha512-OFNPdQAXnQhDSKioX8/XYT6sdUlXwpeMjfd6ApxMJfyZ4GxmLR1xvMERctlYhlHwIiz6CSpBc2+qYKjHGZw4TQ==}
     dependencies:
       compute-gcd: 1.2.1
       validate.io-array: 1.0.6
       validate.io-function: 1.0.2
       validate.io-integer-array: 1.0.0
 
+  /compute-scroll-into-view@3.1.0:
+    resolution: {integrity: sha512-rj8l8pD4bJ1nx+dAkMhV1xB5RuZEyVysfxJqB1pRchh1KVvwOv9b7CGB8ZfjTImVv2oF+sYMUkMZq6Na5Ftmbg==}
+    dev: false
+
   /concat-map@0.0.1:
     resolution: {integrity: sha1-2Klr13/Wjfd5OnMDajug1UBdR3s=}
     dev: true
 
   /conventional-changelog-angular@7.0.0:
     resolution: {integrity: sha512-ROjNchA9LgfNMTTFSIWPzebCwOGFdgkEq45EnvvrmSLvCtAw0HSmrCs7/ty+wAeYUZyNay0YMUNYFTRL72PkBQ==}
     engines: {node: '>=16'}
@@ -4667,14 +5000,20 @@
       split2: 4.2.0
     dev: true
 
   /convert-source-map@2.0.0:
     resolution: {integrity: sha512-Kvp459HrV2FEJ1CAsi1Ku+MY3kasH19TFykTz2xWmMeq6bk2NU3XXvfJ+Q61m0xktWwt+1HSYf3JZsTms3aRJg==}
     dev: true
 
+  /copy-to-clipboard@3.3.3:
+    resolution: {integrity: sha512-2KV8NhB5JqC3ky0r9PMCAZKbUHSwtEo4CwCs0KXgruG43gX5PMqDEBbVU4OUzw2MuAWUfsuFmWvEKG5QRfSnJA==}
+    dependencies:
+      toggle-selection: 1.0.6
+    dev: false
+
   /core-js-compat@3.36.1:
     resolution: {integrity: sha512-Dk997v9ZCt3X/npqzyGdTlq6t7lDBhZwGvV94PKzDArjp7BTRm7WlDAXYd/OWdeFHO8OChQYRJNJvUCqCbrtKA==}
     dependencies:
       browserslist: 4.23.0
     dev: true
 
   /core-util-is@1.0.3:
@@ -4986,14 +5325,25 @@
     engines: {node: '>= 0.4'}
     dependencies:
       call-bind: 1.0.7
       es-errors: 1.3.0
       is-data-view: 1.0.1
     dev: true
 
+  /date-fns@2.30.0:
+    resolution: {integrity: sha512-fnULvOpxnC5/Vg3NCiWelDsLiUc9bRwAPs/+LfTLNvetFCtCTN+yQz15C/fs4AwX1R9K5GLtLfn8QW+dWisaAw==}
+    engines: {node: '>=0.11'}
+    dependencies:
+      '@babel/runtime': 7.24.4
+    dev: false
+
+  /dayjs@1.11.10:
+    resolution: {integrity: sha512-vjAczensTgRcqDERK0SR2XMwsF/tSvnvlv6VcF2GIhg6Sx4yOIt/irsr1RDJsKiIyBzJDpCoXiWWq28MqH2cnQ==}
+    dev: false
+
   /debug@2.6.9:
     resolution: {integrity: sha512-bC7ElrdJaJnPbAP+1EotYvqZsb3ecl5wi6Bfi6BJTUcNowp6cvspg0jXznRTKDjm/E7AdgFBVeAPVMNcKGsHMA==}
     peerDependencies:
       supports-color: '*'
     peerDependenciesMeta:
       supports-color:
         optional: true
@@ -5101,14 +5451,18 @@
   /doctrine@3.0.0:
     resolution: {integrity: sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==}
     engines: {node: '>=6.0.0'}
     dependencies:
       esutils: 2.0.3
     dev: true
 
+  /dom-align@1.12.4:
+    resolution: {integrity: sha512-R8LUSEay/68zE5c8/3BDxiTEvgb4xZTF0RKmAHfiEVN3klfIpXfi2/QCoiWPccVQ0J/ZGdz9OjzL4uJEP/MRAw==}
+    dev: false
+
   /dom-serializer@1.4.1:
     resolution: {integrity: sha512-VHwB3KfrcOOkelEG2ZOfxqLZdfkil8PtJi4P8N2MMXucZq2yLp75ClViUlOVwyoHEDjYU433Aq+5zWP61+RGag==}
     dependencies:
       domelementtype: 2.3.0
       domhandler: 4.3.1
       entities: 2.2.0
 
@@ -6909,14 +7263,20 @@
     resolution: {integrity: sha1-nbe1lJatPzz+8wp1FC0tkwrXJlE=}
     dev: true
 
   /json-stringify-pretty-compact@3.0.0:
     resolution: {integrity: sha512-Rc2suX5meI0S3bfdZuA7JMFBGkJ875ApfVyq2WHELjBiiG22My/l7/8zPpH/CfFVQHuVLd8NLR0nv6vi0BYYKA==}
     dev: true
 
+  /json2mq@0.2.0:
+    resolution: {integrity: sha512-SzoRg7ux5DWTII9J2qkrZrqV1gt+rTaoufMxEzXbS26Uid0NwaJd123HcoB80TgubEppxxIGdNxCx50fEoEWQA==}
+    dependencies:
+      string-convert: 0.2.1
+    dev: false
+
   /json5@2.2.3:
     resolution: {integrity: sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==}
     engines: {node: '>=6'}
     hasBin: true
 
   /jsonfile@6.1.0:
     resolution: {integrity: sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==}
@@ -7289,14 +7649,18 @@
 
   /mkdirp@1.0.4:
     resolution: {integrity: sha512-vVqVZQyf3WLx2Shd0qJ9xuvqgAyKPLAiqITEtqW0oIUjzo3PePDd6fW9iFz30ef7Ysp/oiWqbhszeGWW2T6Gzw==}
     engines: {node: '>=10'}
     hasBin: true
     dev: true
 
+  /moment@2.30.1:
+    resolution: {integrity: sha512-uEmtNhbDOrWPFS+hdjFCBfy9f2YoyzRpwcl+DqpC6taX21FzsTLQVbMV/W7PzNSX6x/bhC1zA3c2UQ5NzH6how==}
+    dev: false
+
   /ms@2.0.0:
     resolution: {integrity: sha1-VgiurfwAvmwpAd9fmGF4jeDVl8g=}
     dev: true
 
   /ms@2.1.2:
     resolution: {integrity: sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==}
     dev: true
@@ -7743,14 +8107,22 @@
     resolution: {integrity: sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==}
     engines: {node: '>=6'}
 
   /pure-rand@6.0.4:
     resolution: {integrity: sha512-LA0Y9kxMYv47GIPJy6MI84fqTd2HmYZI83W/kM/SkKfDlajnZYfmXFTxkbY+xSBPkLJxltMa9hIkmdc29eguMA==}
     dev: true
 
+  /qrcode.react@3.1.0(react@18.2.0):
+    resolution: {integrity: sha512-oyF+Urr3oAMUG/OiOuONL3HXM+53wvuH3mtIWQrYmsXoAq0DkvZp2RYUWFSMFtbdOpuS++9v+WAkzNVkMlNW6Q==}
+    peerDependencies:
+      react: ^16.8.0 || ^17.0.0 || ^18.0.0
+    dependencies:
+      react: 18.2.0
+    dev: false
+
   /querystringify@2.2.0:
     resolution: {integrity: sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==}
 
   /queue-microtask@1.2.3:
     resolution: {integrity: sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==}
     dev: true
 
@@ -7766,14 +8138,576 @@
 
   /randombytes@2.1.0:
     resolution: {integrity: sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==}
     dependencies:
       safe-buffer: 5.2.1
     dev: true
 
+  /rc-align@4.0.15(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-wqJtVH60pka/nOX7/IspElA8gjPNQKIx/ZqJ6heATCkXpe1Zg4cPVrMD2vC96wjsFFL8WsmhPbx9tdMo1qqlIA==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      dom-align: 1.12.4
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+      resize-observer-polyfill: 1.5.1
+    dev: false
+
+  /rc-cascader@3.24.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-RgKuYgEGPx+6wCgguYFHjMsDZdCyydZd58YJRCfYQ8FObqLnZW0x/vUcEyPjhWIj1EhjV958IcR+NFPDbbj9kg==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      array-tree-filter: 2.1.0
+      classnames: 2.5.1
+      rc-select: 14.13.1(react-dom@18.2.0)(react@18.2.0)
+      rc-tree: 5.8.5(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-checkbox@3.2.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-8inzw4y9dAhZmv/Ydl59Qdy5tdp9CKg4oPVcRigi+ga/yKPZS5m5SyyQPtYSgbcqHRYOdUhiPSeKfktc76du1A==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-collapse@3.7.3(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-60FJcdTRn0X5sELF18TANwtVi7FtModq649H11mYF1jh83DniMoM4MqY627sEKRCTm4+WXfGDcB7hY5oW6xhyw==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-dialog@9.4.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-AScCexaLACvf8KZRqCPz12BJ8olszXOS4lKlkMyzDQHS1m0zj1KZMYgmMCh39ee0Dcv8kyrj8mTqxuLyhH+QuQ==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/portal': 1.1.2(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-drawer@7.1.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-nBE1rF5iZvpavoyqhSSz2mk/yANltA7g3aF0U45xkx381n3we/RKs9cJfNKp9mSWCedOKWt9FLEwZDaAaOGn2w==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/portal': 1.1.2(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-dropdown@4.2.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-odM8Ove+gSh0zU27DUj5cG1gNKg7mLWBYzB5E4nNLrLwBmYEgYP43vHKDGOVZcJSVElQBI0+jTQgjnq0NfLjng==}
+    peerDependencies:
+      react: '>=16.11.0'
+      react-dom: '>=16.11.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-field-form@1.44.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-el7w87fyDUsca63Y/s8qJcq9kNkf/J5h+iTdqG5WsSHLH0e6Usl7QuYSmSVzJMgtp40mOVZIY/W/QP9zwrp1FA==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      async-validator: 4.2.5
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-image@7.6.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-tL3Rvd1sS+frZQ01i+tkeUPaOeFz2iG9/scAt/Cfs0hyCRVA/w0Pu1J/JxIX8blalvmHE0bZQRYdOmRAzWu4Hg==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/portal': 1.1.2(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-dialog: 9.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-input-number@9.0.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-RfcDBDdWFFetouWFXBA+WPEC8LzBXyngr9b+yTLVIygfFu7HiLRGn/s/v9wwno94X7KFvnb28FNynMGj9XJlDQ==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/mini-decimal': 1.1.0
+      classnames: 2.5.1
+      rc-input: 1.4.5(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-input@1.4.5(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-AjzykhwnwYTRSwwgCu70CGKBIAv6bP2nqnFptnNTprph/TF1BAs0Qxl91mie/BR6n827WIJB6ZjaRf9iiMwAfw==}
+    peerDependencies:
+      react: '>=16.0.0'
+      react-dom: '>=16.0.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-mentions@2.11.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-upb4AK1SRFql7qGnbLEvJqLMugVVIyjmwBJW9L0eLoN9po4JmJZaBzmKA4089fNtsU8k6l/tdZiVafyooeKnLw==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-input: 1.4.5(react-dom@18.2.0)(react@18.2.0)
+      rc-menu: 9.13.0(react-dom@18.2.0)(react@18.2.0)
+      rc-textarea: 1.6.3(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-menu@9.13.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-1l8ooCB3HcYJKCltC/s7OxRKRjgymdl9htrCeGZcXNaMct0RxZRK6OPV3lPhVksIvAGMgzPd54ClpZ5J4b8cZA==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-overflow: 1.3.2(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-motion@2.9.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-XIU2+xLkdIr1/h6ohPZXyPBMvOmuyFZQ/T0xnawz+Rh+gh4FINcnZmMT5UTIj6hgI0VLDjTaPeRd+smJeSPqiQ==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-notification@5.4.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-li19y9RoYJciF3WRFvD+DvWS70jdL8Fr+Gfb/OshK+iY6iTkwzoigmSIp76/kWh5tF5i/i9im12X3nsF85GYdA==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-overflow@1.3.2(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-nsUm78jkYAoPygDAcGZeC2VwIg/IBGSodtOY3pMof4W3M9qRJgqaDYm03ZayHlde3I6ipliAxbN0RUcGf5KOzw==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-pagination@4.0.4(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-GGrLT4NgG6wgJpT/hHIpL9nELv27A1XbSZzECIuQBQTVSf4xGKxWr6I/jhpRPauYEWEbWVw22ObG6tJQqwJqWQ==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-picker@2.7.6(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-H9if/BUJUZBOhPfWcPeT15JUI3/ntrG9muzERrXDkSoWmDj4yzmBvumozpxYrHwjcKnjyDGAke68d+whWwvhHA==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      date-fns: 2.30.0
+      dayjs: 1.11.10
+      moment: 2.30.1
+      rc-trigger: 5.3.4(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+      shallowequal: 1.1.0
+    dev: false
+
+  /rc-picker@4.3.2(dayjs@1.11.10)(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-2NtobLxG2YqllXn4YczbupgIH6PSqzjCfFCnGlgPIY9k0HZti8WmBPjS1OD9JKQl+Tdg0pMVUeTEc07y4X9ZRQ==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      date-fns: '>= 2.x'
+      dayjs: '>= 1.x'
+      luxon: '>= 3.x'
+      moment: '>= 2.x'
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    peerDependenciesMeta:
+      date-fns:
+        optional: true
+      dayjs:
+        optional: true
+      luxon:
+        optional: true
+      moment:
+        optional: true
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      dayjs: 1.11.10
+      rc-overflow: 1.3.2(react-dom@18.2.0)(react@18.2.0)
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-progress@4.0.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-oofVMMafOCokIUIBnZLNcOZFsABaUw8PPrf1/y0ZBvKZNpOiu5h4AO9vv11Sw0p4Hb3D0yGWuEattcQGtNJ/aw==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-rate@2.12.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-g092v5iZCdVzbjdn28FzvWebK2IutoVoiTeqoLTj9WM7SjA/gOJIw5/JFZMRyJYYVe1jLAU2UhAfstIpCNRozg==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-resize-observer@1.4.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-PnMVyRid9JLxFavTjeDXEXo65HCRqbmLBw9xX9gfC4BZiSzbLXKzW3jPz+J0P71pLbD5tBMTT+mkstV5gD0c9Q==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+      resize-observer-polyfill: 1.5.1
+    dev: false
+
+  /rc-segmented@2.3.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-I3FtM5Smua/ESXutFfb8gJ8ZPcvFR+qUgeeGFQHBOvRiRKyAk4aBE5nfqrxXx+h8/vn60DQjOt6i4RNtrbOobg==}
+    peerDependencies:
+      react: '>=16.0.0'
+      react-dom: '>=16.0.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-select@14.13.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-A1VHqjIOemxLnUGRxLGVqXBs8jGcJemI5NXxOJwU5PQc1wigAu1T4PRLgMkTPDOz8gPhlY9dwsPzMgakMc2QjQ==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '*'
+      react-dom: '*'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-overflow: 1.3.2(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      rc-virtual-list: 3.11.4(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-slider@10.5.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-xiYght50cvoODZYI43v3Ylsqiw14+D7ELsgzR40boDZaya1HFa1Etnv9MDkQE8X/UrXAffwv2AcNAhslgYuDTw==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-steps@6.0.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-lKHL+Sny0SeHkQKKDJlAjV5oZ8DwCdS2hFhAkIjuQt1/pB81M0cA0ErVFdHq9+jmPmFw1vJB2F5NBzFXLJxV+g==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-switch@4.1.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-TI8ufP2Az9oEbvyCeVE4+90PDSljGyuwix3fV58p7HV2o4wBnVToEyomJRVyTaZeqNPAp+vqeo4Wnj5u0ZZQBg==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-table@7.45.4(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-6aSbGrnkN2GLSt3s1x+wa4f3j/VEgg1uKPpaLY5qHH1/nFyreS2V7DFJ0TfUb18allf2FQl7oVYEjTixlBXEyQ==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/context': 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      rc-virtual-list: 3.11.4(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-tabs@14.1.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-5nOr9PVpJy2SWHTLgv1+kESDOb0tFzl0cYU9r9d8LfL0Wg9i/n1B558rmkxdQHgBwMqxmwoyPSAbQROxMQe8nw==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-dropdown: 4.2.0(react-dom@18.2.0)(react@18.2.0)
+      rc-menu: 9.13.0(react-dom@18.2.0)(react@18.2.0)
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-textarea@1.6.3(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-8k7+8Y2GJ/cQLiClFMg8kUXOOdvcFQrnGeSchOvI2ZMIVvX5a3zQpLxoODL0HTrvU63fPkRmMuqaEcOF9dQemA==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-input: 1.4.5(react-dom@18.2.0)(react@18.2.0)
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-tooltip@6.2.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-iS/3iOAvtDh9GIx1ulY7EFUXUtktFccNLsARo3NPgLf0QW9oT0w3dA9cYWlhqAKmD+uriEwdWz1kH0Qs4zk2Aw==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      '@rc-component/trigger': 2.1.1(react-dom@18.2.0)(react@18.2.0)
+      classnames: 2.5.1
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-tree-select@5.19.0(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-f4l5EsmSGF3ggj76YTzKNPY9SnXfFaer7ZccTSGb3urUf54L+cCqyT+UsPr+S5TAr8mZSxJ7g3CgkCe+cVQ6sw==}
+    peerDependencies:
+      react: '*'
+      react-dom: '*'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-select: 14.13.1(react-dom@18.2.0)(react@18.2.0)
+      rc-tree: 5.8.5(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-tree@5.8.5(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-PRfcZtVDNkR7oh26RuNe1hpw11c1wfgzwmPFL0lnxGnYefe9lDAO6cg5wJKIAwyXFVt5zHgpjYmaz0CPy1ZtKg==}
+    engines: {node: '>=10.x'}
+    peerDependencies:
+      react: '*'
+      react-dom: '*'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      rc-virtual-list: 3.11.4(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-trigger@5.3.4(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-mQv+vas0TwKcjAO2izNPkqR4j86OemLRmvL2nOzdP9OWNWA1ivoTt5hzFqYNW9zACwmTezRiN8bttrC7cZzYSw==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-align: 4.0.15(react-dom@18.2.0)(react@18.2.0)
+      rc-motion: 2.9.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-upload@4.5.2(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-QO3ne77DwnAPKFn0bA5qJM81QBjQi0e0NHdkvpFyY73Bea2NfITiotqJqVjHgeYPOJu5lLVR32TNGP084aSoXA==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
+  /rc-util@5.39.1(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-OW/ERynNDgNr4y0oiFmtes3rbEamXw7GHGbkbNd9iRr7kgT03T6fT0b9WpJ3mbxKhyOcAHnGcIoh5u/cjrC2OQ==}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+      react-is: 18.2.0
+    dev: false
+
+  /rc-virtual-list@3.11.4(react-dom@18.2.0)(react@18.2.0):
+    resolution: {integrity: sha512-NbBi0fvyIu26gP69nQBiWgUMTPX3mr4FcuBQiVqagU0BnuX8WQkiivnMs105JROeuUIFczLrlgUhLQwTWV1XDA==}
+    engines: {node: '>=8.x'}
+    peerDependencies:
+      react: '>=16.9.0'
+      react-dom: '>=16.9.0'
+    dependencies:
+      '@babel/runtime': 7.24.4
+      classnames: 2.5.1
+      rc-resize-observer: 1.4.0(react-dom@18.2.0)(react@18.2.0)
+      rc-util: 5.39.1(react-dom@18.2.0)(react@18.2.0)
+      react: 18.2.0
+      react-dom: 18.2.0(react@18.2.0)
+    dev: false
+
   /react-dom@18.2.0(react@18.2.0):
     resolution: {integrity: sha512-6IMTriUmvsjHUjNtEDudZfuDQUoWXVxKHhlEGSk81n4YFS+r/Kl99wXiwlVXtPBtJenozv2P+hxDsw9eA7Xo6g==}
     peerDependencies:
       react: ^18.2.0
     dependencies:
       loose-envify: 1.4.0
       react: 18.2.0
@@ -7891,15 +8825,14 @@
 
   /regenerate@1.4.2:
     resolution: {integrity: sha512-zrceR/XhGYU/d/opr2EKO7aRHUeiBI8qjtfHqADTwZd6Szfy16la6kqD0MIUs5z5hx6AaKa+PixpPrR289+I0A==}
     dev: true
 
   /regenerator-runtime@0.14.1:
     resolution: {integrity: sha512-dYnhHh0nJoMfnkZs6GmmhFknAGRrLznOu5nc9ML+EJxGvrx6H7teuevqVqCuPcPK//3eDrrjQhehXVx9cnkGdw==}
-    dev: true
 
   /regenerator-transform@0.15.2:
     resolution: {integrity: sha512-hfMp2BoF0qOk3uc5V20ALGDS2ddjQaLrdl7xrGXvAIow7qeWRM2VA2HuCHkUKk9slq3VwEwLNK3DFBqDfPGYtg==}
     dependencies:
       '@babel/runtime': 7.24.1
     dev: true
 
@@ -7955,14 +8888,18 @@
   /require-from-string@2.0.2:
     resolution: {integrity: sha512-Xf0nWe6RseziFMu+Ap9biiUbmplq6S9/p+7w7YXP/JBHhrUDDUhwa+vANyubuqfZWTveU//DYVGsDG7RKL/vEw==}
     engines: {node: '>=0.10.0'}
 
   /requires-port@1.0.0:
     resolution: {integrity: sha1-kl0mAdOaxIXgkc8NpcbmlNw9yv8=}
 
+  /resize-observer-polyfill@1.5.1:
+    resolution: {integrity: sha512-LwZrotdHOo12nQuZlHEmtuXdqGoOD0OhaxopaNFxWzInpEgaLWoVuAMbTzixuosCx2nEG58ngzW3vxdWoxIgdg==}
+    dev: false
+
   /resolve-cwd@3.0.0:
     resolution: {integrity: sha512-OrZaX2Mb+rJCpH/6CpSqt9xFVpN++x01XnN2ie9g6P5/3xelLAkXWVADpdz1IHD/KFfEXyE6V0U01OQ3UO2rEg==}
     engines: {node: '>=8'}
     dependencies:
       resolve-from: 5.0.0
     dev: true
 
@@ -8108,14 +9045,20 @@
     dependencies:
       '@types/json-schema': 7.0.15
       ajv: 8.12.0
       ajv-formats: 2.1.1(ajv@8.12.0)
       ajv-keywords: 5.1.0(ajv@8.12.0)
     dev: true
 
+  /scroll-into-view-if-needed@3.1.0:
+    resolution: {integrity: sha512-49oNpRjWRvnU8NyGVmUaYG4jtTkNonFZI86MmGRDqBphEK2EXT9gdEUoQPZhuBM8yWHxCWbobltqYO5M4XrUvQ==}
+    dependencies:
+      compute-scroll-into-view: 3.1.0
+    dev: false
+
   /semver@5.7.2:
     resolution: {integrity: sha512-cBznnQ9KjJqU67B52RMC65CMarK2600WFnbkcaiwWq3xy/5haFJlshgnpjovMVJ+Hff49d8GEn0b87C5pDQ10g==}
     hasBin: true
     dev: true
 
   /semver@6.3.1:
     resolution: {integrity: sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==}
@@ -8161,14 +9104,18 @@
   /shallow-clone@3.0.1:
     resolution: {integrity: sha512-/6KqX+GVUdqPuPPd2LxDDxzX6CAbjJehAAOKlNpqqUpAqPM6HeL8f+o3a+JsyGjn2lv0WY8UsTgUJjU9Ok55NA==}
     engines: {node: '>=8'}
     dependencies:
       kind-of: 6.0.3
     dev: true
 
+  /shallowequal@1.1.0:
+    resolution: {integrity: sha512-y0m1JoUZSlPAjXVtPPW70aZWfIL/dSP7AFkRnniLCrK/8MDKog3TySTBmckD+RObVxH0v4Tox67+F14PdED2oQ==}
+    dev: false
+
   /shebang-command@1.2.0:
     resolution: {integrity: sha1-RKrGW2lbAzmJaMOfNj/uXer98eo=}
     engines: {node: '>=0.10.0'}
     dependencies:
       shebang-regex: 1.0.0
     dev: true
 
@@ -8332,14 +9279,18 @@
   /stack-utils@2.0.6:
     resolution: {integrity: sha512-XlkWvfIm6RmsWtNJx+uqtKLS8eqFbxUg0ZzLXqY0caEy9l7hruX8IpiDnjsLavoBgqCCR71TqWO8MaXYheJ3RQ==}
     engines: {node: '>=10'}
     dependencies:
       escape-string-regexp: 2.0.0
     dev: true
 
+  /string-convert@0.2.1:
+    resolution: {integrity: sha512-u/1tdPl4yQnPBjnVrmdLo9gtuLvELKsAoRapekWggdiQNvvvum+jYF329d84NAa660KQw7pB2n36KrIKVoXa3A==}
+    dev: false
+
   /string-length@4.0.2:
     resolution: {integrity: sha512-+l6rNN5fYHNhZZy41RXsYptCjA2Igmq4EG7kZAYFQI1E1VTXarr6ZPXBg6eq7Y6eK4FEhY6AJlyuFIb/v/S0VQ==}
     engines: {node: '>=10'}
     dependencies:
       char-regex: 1.0.2
       strip-ansi: 6.0.1
     dev: true
@@ -8550,14 +9501,18 @@
       table: 6.8.1
       write-file-atomic: 5.0.1
     transitivePeerDependencies:
       - supports-color
       - typescript
     dev: true
 
+  /stylis@4.3.1:
+    resolution: {integrity: sha512-EQepAV+wMsIaGVGX1RECzgrcqRRU/0sYOHkeLsZ3fzHaHXZy4DaOOX0vOlGQdlsjkh3mFHAIlVimpwAs4dslyQ==}
+    dev: false
+
   /supports-color@5.5.0:
     resolution: {integrity: sha512-QjVjwdXIt408MIiAqCX4oUKsgU2EqAGzs2Ppkm4aQYbjm+ZEWEcW4SfFNTr4uMNZma0ey4f5lgLrkB0aX0QMow==}
     engines: {node: '>=4'}
     dependencies:
       has-flag: 3.0.0
     dev: true
 
@@ -8679,14 +9634,19 @@
     engines: {node: '>=8'}
     dev: true
 
   /text-table@0.2.0:
     resolution: {integrity: sha1-f17oI66AUgfACvLfSoTsP8+lcLQ=}
     dev: true
 
+  /throttle-debounce@5.0.0:
+    resolution: {integrity: sha512-2iQTSgkkc1Zyk0MeVrt/3BvuOXYPl/R8Z0U2xxo9rjwNciaHDG3R+Lm6dh4EeUci49DanvBnuqI6jshoQQRGEg==}
+    engines: {node: '>=12.22'}
+    dev: false
+
   /through2@4.0.2:
     resolution: {integrity: sha512-iOqSav00cVxEEICeD7TjLB1sueEL+81Wpzp2bY17uZjZN0pWZPuo4suZ/61VujxmqSGFfgOcNuTZ85QJwNZQpw==}
     dependencies:
       readable-stream: 3.6.2
     dev: true
 
   /through@2.3.8:
@@ -8705,14 +9665,18 @@
   /to-regex-range@5.0.1:
     resolution: {integrity: sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==}
     engines: {node: '>=8.0'}
     dependencies:
       is-number: 7.0.0
     dev: true
 
+  /toggle-selection@1.0.6:
+    resolution: {integrity: sha512-BiZS+C1OS8g/q2RRbJmy59xpyghNBqrr6k5L/uKBGRsTfxmu3ffiRnd8mlGPUVayg8pvfi5urfnu8TU7DVOkLQ==}
+    dev: false
+
   /topojson-client@3.1.0:
     resolution: {integrity: sha512-605uxS6bcYxGXw9qi62XyrV6Q3xwbndjachmNxu8HWTtVPxZfEJN9fd/SZS1Q54Sn2y0TMyMxFj/cJINqGHrKw==}
     hasBin: true
     dependencies:
       commander: 2.20.3
     dev: true
 
@@ -8966,14 +9930,22 @@
 
   /url-parse@1.5.10:
     resolution: {integrity: sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==}
     dependencies:
       querystringify: 2.2.0
       requires-port: 1.0.0
 
+  /use-sync-external-store@1.2.0(react@18.2.0):
+    resolution: {integrity: sha512-eEgnFxGQ1Ife9bzYs6VLi8/4X6CObHMw9Qr9tPY43iKwsPw8xE8+EFsf/2cFZ5S3esXgpWgtSCtLNS41F+sKPA==}
+    peerDependencies:
+      react: ^16.8.0 || ^17.0.0 || ^18.0.0
+    dependencies:
+      react: 18.2.0
+    dev: false
+
   /util-deprecate@1.0.2:
     resolution: {integrity: sha1-RQ1Nyfpw3nMnYvvS1KKJgUGaDM8=}
     dev: true
 
   /util@0.10.4:
     resolution: {integrity: sha512-0Pm9hTQ3se5ll1XihRic3FDIku70C+iHUdT/W926rSgHV5QgXsYbKZN8MSC3tJtSkhuROzvsQjAaFENRXr+19A==}
     dependencies:
@@ -9726,7 +10698,26 @@
     dependencies:
       lib0: 0.2.93
 
   /yocto-queue@0.1.0:
     resolution: {integrity: sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==}
     engines: {node: '>=10'}
     dev: true
+
+  /zustand@4.5.2(react@18.2.0):
+    resolution: {integrity: sha512-2cN1tPkDVkwCy5ickKrI7vijSjPksFRfqS6237NzT0vqSsztTNnQdHw9mmN7uBdk3gceVXU0a+21jFzFzAc9+g==}
+    engines: {node: '>=12.7.0'}
+    peerDependencies:
+      '@types/react': '>=16.8'
+      immer: '>=9.0.6'
+      react: '>=16.8'
+    peerDependenciesMeta:
+      '@types/react':
+        optional: true
+      immer:
+        optional: true
+      react:
+        optional: true
+    dependencies:
+      react: 18.2.0
+      use-sync-external-store: 1.2.0(react@18.2.0)
+    dev: false
```

### Comparing `neopyter-0.2.1/tsconfig.json` & `neopyter-0.2.2/tsconfig.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'include'": "{insert: [(1, 'src/**/*.tsx')]}"}*

```diff
@@ -22,10 +22,11 @@
         "skipLibCheck": true,
         "strict": true,
         "strictNullChecks": true,
         "target": "ES2018"
     },
     "include": [
         "src/**/*.ts",
+        "src/**/*.tsx",
         "src/**/*.d.ts"
     ]
 }
```

### Comparing `neopyter-0.2.1/after/queries/python/highlights.scm` & `neopyter-0.2.2/after/queries/python/highlights.scm`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/after/queries/python/injections.scm` & `neopyter-0.2.2/after/queries/python/injections.scm`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/after/queries/python/textobjects.scm` & `neopyter-0.2.2/after/queries/python/textobjects.scm`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/cell_magic.png` & `neopyter-0.2.2/doc/cell_magic.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/communication_direct.png` & `neopyter-0.2.2/doc/communication_direct.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/communication_proxy.png` & `neopyter-0.2.2/doc/communication_proxy.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/completion.png` & `neopyter-0.2.2/doc/completion.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/example.ju.py` & `neopyter-0.2.2/doc/example.ju.py`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/line_magic.png` & `neopyter-0.2.2/doc/line_magic.png`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/doc/neopyter.txt` & `neopyter-0.2.2/doc/neopyter.txt`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter.lua` & `neopyter-0.2.2/lua/neopyter.lua`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     filename_mapper = function(ju_path)
         local ipynb_path = ju_path:gsub("%.ju%.%w+", ".ipynb")
         return ipynb_path
     end,
 
     auto_attach = true,
     auto_connect = true,
-    mode = "proxy",
+    mode = "direct",
     jupyter = {
         auto_activate_file = true,
         -- Always scroll to the current cell.
         scroll = {
             enable = true,
             mode = "always", -- "always" or "invisible"
             step = 0.5,
```

### Comparing `neopyter-0.2.1/lua/neopyter/asyncwrap.lua` & `neopyter-0.2.2/lua/neopyter/asyncwrap.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/cmp.lua` & `neopyter-0.2.2/lua/neopyter/cmp.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/health.lua` & `neopyter-0.2.2/lua/neopyter/health.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/highlight.lua` & `neopyter-0.2.2/lua/neopyter/highlight.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/textobjects.lua` & `neopyter-0.2.2/lua/neopyter/textobjects.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/utils.lua` & `neopyter-0.2.2/lua/neopyter/utils.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/jupyter/jupyterlab.lua` & `neopyter-0.2.2/lua/neopyter/jupyter/jupyterlab.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/jupyter/notebook.lua` & `neopyter-0.2.2/lua/neopyter/jupyter/notebook.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/rpc/asyncclient.lua` & `neopyter-0.2.2/lua/neopyter/rpc/asyncclient.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/rpc/baseclient.lua` & `neopyter-0.2.2/lua/neopyter/rpc/baseclient.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/rpc/blockclient.lua` & `neopyter-0.2.2/lua/neopyter/rpc/blockclient.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/rpc/msgpack.lua` & `neopyter-0.2.2/lua/neopyter/rpc/msgpack.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/lua/neopyter/rpc/wsserverclient.lua` & `neopyter-0.2.2/lua/neopyter/rpc/wsserverclient.lua`

 * *Files 7% similar despite different names*

```diff
@@ -38,34 +38,38 @@
         if not restart_server then
             return
         end
         self.server:close()
     end
     local host, port = utils.parse_address(self.address)
     self.server = websocket.Server:new({ host = host, port = port })
-    self.server:listen({
+    local success, error = pcall(self.server.listen, self.server, {
         on_connect = function(connect)
             if self.single_connection ~= nil then
-                logger.warn("server listening and client exists, but another client income")
-                self.single_connection:close()
+                logger.warn("server listening and client exists, but another client incoming")
+                utils.notify_warn("There are multiple lab extension connections at same time, please check if multiple tagbs are open")
+                connect:close()
             end
             self.single_connection = connect
             self.single_connection:attach({
                 on_text = function(text)
-                    self:handle_response(vim.base64.decode(text))
+                    self:handle_response(text)
                 end,
                 on_disconnect = function()
                     self.single_connection = nil
                 end,
             })
         end,
         on_disconnect = function()
             self:disconnect()
         end,
     })
+    if not success then
+        utils.notify_warn(error)
+    end
 end
 
 ---disconnect connect
 function WSServerClient:disconnect()
     if self.single_connection then
         self.single_connection:close()
         self.single_connection = nil
@@ -126,18 +130,20 @@
     end
 end
 
 ---handle rpc response
 ---@param data string
 ---@package
 function WSServerClient:handle_response(data)
-    local status, msg = pcall(vim.mpack.decode, data)
-    assert(status, vim.inspect(msg) .. data)
-    if status == false then
+    local mpack = vim.base64.decode(data)
+    local status, msg = pcall(vim.mpack.decode, mpack)
+    if not status then
         logger.warn("parse mpack error, reset request pool")
+        -- assert(status, string.format("%s: recevied data.length=%s, mpack.length=%s, msg=[%s]", vim.inspect(msg), #data, #mpack, mpack))
+        utils.notify_error(msg)
         self:reset_request()
         return
     end
     if #msg == 4 and msg[1] == 1 then
         local msgid, error, result = msg[2], msg[3], msg[4]
         local callback = self.request_pool[msgid]
         self.request_pool[msgid] = nil
@@ -153,15 +159,15 @@
         )
         if error == vim.NIL then
             callback(true, result)
         else
             callback(false, error)
         end
     else
-        assert(false, "msgpack rpc response spec error, msg=" .. data)
+        assert(false, "msgpack rpc response spec error, msg=" .. mpack)
     end
 end
 
 function WSServerClient:notify(event, ...) end
 
 function WSServerClient:reset_request()
     for _, fun in pairs(self.request_pool) do
```

### Comparing `neopyter-0.2.1/lua-tests/neopyter/utils_spec.lua` & `neopyter-0.2.2/lua-tests/neopyter/utils_spec.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/neopyter/__init__.py` & `neopyter-0.2.2/neopyter/__init__.py`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/neopyter/handler.py` & `neopyter-0.2.2/neopyter/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Union, Optional, Awaitable
 import base64
 
 from .msgpack_queue import labextension_queue, client_queue
 from .tcp_server import tcpServer
 
 
-settings = {"mode": "proxy", "host": "127.0.0.1", "port": 9001}
+settings = {"mode": "direct", "host": "127.0.0.1", "port": 9001}
 
 
 class ForwardWebsocketHandler(WebSocketHandler):
     def open(self, *args: str, **kwargs: str) -> Optional[Awaitable[None]]:
         print("Websocket opened for lab extension")
         if settings["mode"] == "direct":
             print("mode is direct, cann't connect jupyter server websocket")
@@ -77,51 +77,56 @@
         settings = tornado.escape.json_decode(self.request.body)
         mode = settings.get("mode", "proxy")
 
         host = (settings.get("ip", "") or "").strip().split(",")
         while "" in host:
             host.remove("")
 
-        port = settings["port"]
+        port = settings.get("port", 9001)
 
         print("-------------debug-------------------")
         settings["mode"] = mode
         settings["host"] = host
         settings["port"] = port
         print(mode, host, port, tcpServer.is_running)
         if mode == "direct":
             if tcpServer.is_running:
                 asyncio.create_task(tcpServer.stop())
+                print("success, tcp server is running, shutdown it")
                 return self.finish(
                     {
                         "code": 0,
                         "message": "success, tcp server is running, shutdown it",
                     }
                 )
+            print("success, tcp server is shutdown")
             return self.finish(
                 {
                     "code": 0,
                     "message": "success, tcp server is shutdown",
                 }
             )
-        if host == tcpServer.host and port == tcpServer.port:
+
+        if host == tcpServer.host and port == tcpServer.port and tcpServer.is_running:
+            print("no update, don't restart server")
             return self.finish(
                 {
                     "code": 0,
-                    "message": "success, don't restart server",
+                    "message": "no update, don't restart server",
                 }
             )
 
         tcpServer.host = host
         tcpServer.port = port
         asyncio.create_task(tcpServer.start())
+        print("start tcpserver")
         return self.finish(
             {
                 "code": 0,
-                "message": "success",
+                "message": "start/restart tcpserver",
             }
         )
 
 
 def setup_handlers(web_app: ServerWebApplication):
     base_url = web_app.settings["base_url"]
     host_pattern = ".*$"
```

### Comparing `neopyter-0.2.1/neopyter/tcp_server.py` & `neopyter-0.2.2/neopyter/tcp_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     @property
     def is_running(self) -> bool:
         return self.server is not None
 
     async def start(self):
         # support update?
         if self.server:
-            print("Stop old server")
+            print("stop old server")
             await self.stop()
         host = set.union(self.builtinHost, self.host)
         print("resolved host:", host)
         self.server = await asyncio.start_server(
             lambda r, w: self.client_connected(r, w), list(host), self.port
         )
         addrs = ", ".join(str(sock.getsockname()) for sock in self.server.sockets)
```

### Comparing `neopyter-0.2.1/neopyter/labextension/package.json` & `neopyter-0.2.2/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9627926421404682%*

 * *Differences: {"'dependencies'": "{'@rjsf/antd': '^5.18.2', '@rjsf/core': '^5.18.2', '@rjsf/utils': '^5.18.2', "*

 * *                   "'@rjsf/validator-ajv8': '^5.18.2', 'antd': '^5.16.2', 'zustand': '^4.5.2'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -9,15 +9,21 @@
     "dependencies": {
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.2.5",
         "@jupyterlab/logconsole": "^4.1.5",
         "@jupyterlab/notebook": "^4.1.5",
         "@lumino/widgets": "^2.3.1",
         "@msgpack/msgpack": "3.0.0-beta2",
-        "remeda": "^1.55.0"
+        "@rjsf/antd": "^5.18.2",
+        "@rjsf/core": "^5.18.2",
+        "@rjsf/utils": "^5.18.2",
+        "@rjsf/validator-ajv8": "^5.18.2",
+        "antd": "^5.16.2",
+        "remeda": "^1.55.0",
+        "zustand": "^4.5.2"
     },
     "description": "A JupyterLab extension. Integrate JupyterLab and Neovim",
     "devDependencies": {
         "@commitlint/cli": "^18.6.1",
         "@commitlint/config-conventional": "^18.6.3",
         "@jupyterlab/builder": "^4.1.5",
         "@jupyterlab/completer": "^4.1.5",
@@ -54,19 +60,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/SUSTech-data/neopyter",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.dfbe5e3084dd43118cf8.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "neopyter/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -140,12 +141,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1",
+    "version": "0.2.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `neopyter-0.2.1/neopyter/labextension/schemas/neopyter/labplugin.json` & `neopyter-0.2.2/neopyter/labextension/schemas/neopyter/labplugin.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7604166666666666%*

 * *Differences: {"'definitions'": "{'mode': {'type': 'string'}}",*

 * * "'dependencies'": "OrderedDict([('mode', OrderedDict([('oneOf', [OrderedDict([('properties', "*

 * *                   "OrderedDict([('mode', OrderedDict([('enum', ['direct'])]))]))]), "*

 * *                   "OrderedDict([('properties', OrderedDict([('mode', OrderedDict([('enum', "*

 * *                   "['proxy'])])), ('ip', OrderedDict([('title', 'IP'), ('description', 'For "*

 * *                   "`proxy` mode, this is the IP of the host where jupyter server is locat […]*

```diff
@@ -1,42 +1,66 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": false,
     "definitions": {
         "ip": {
             "type": "string"
         },
         "mode": {
             "enum": [
                 "proxy",
                 "direct"
-            ]
+            ],
+            "type": "string"
         },
         "port": {
             "type": "number"
         }
     },
+    "dependencies": {
+        "mode": {
+            "oneOf": [
+                {
+                    "properties": {
+                        "mode": {
+                            "enum": [
+                                "direct"
+                            ]
+                        }
+                    }
+                },
+                {
+                    "properties": {
+                        "ip": {
+                            "$ref": "#/definitions/ip",
+                            "default": "127.0.0.1",
+                            "description": "For `proxy` mode, this is the IP of the host where jupyter server is located",
+                            "title": "IP"
+                        },
+                        "mode": {
+                            "enum": [
+                                "proxy"
+                            ]
+                        },
+                        "port": {
+                            "$ref": "#/definitions/port",
+                            "default": 9001,
+                            "title": "Port"
+                        }
+                    }
+                }
+            ]
+        }
+    },
     "description": "A JupyterLab extension. Integrate JupyterLab and Neovim",
     "jupyter.lab.setting-icon": "ui-components:neopyter",
     "jupyter.lab.setting-icon-label": "Neopyter",
     "properties": {
-        "ip": {
-            "$ref": "#/definitions/ip",
-            "default": "127.0.0.1",
-            "description": "For `proxy` mode, this is the IP of the host where jupyter server is located; For `direct` mode, this is the IP of the host where nvim is located ",
-            "title": "IP"
-        },
         "mode": {
             "$ref": "#/definitions/mode",
             "default": "direct",
-            "description": "Different work mode determine different methods of communication arcitecture. The `proxy` mode will communicate through jupyter server, while the `direct` mode will communicate directly with nvim",
-            "title": "Neopyter work mode"
-        },
-        "port": {
-            "$ref": "#/definitions/port",
-            "default": 9001,
-            "title": "Port"
+            "description": "Different work mode determine different methods of communication. The `proxy` mode will communicate through jupyter server, while the `direct` mode will communicate directly with nvim",
+            "title": "Neopyter mode"
         }
     },
     "title": "Neopyter",
     "type": "object"
 }
```

### Comparing `neopyter-0.2.1/neopyter/labextension/schemas/neopyter/package.json.orig` & `neopyter-0.2.2/neopyter/labextension/schemas/neopyter/package.json.orig`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9682274247491639%*

 * *Differences: {"'dependencies'": "{'@rjsf/antd': '^5.18.2', '@rjsf/core': '^5.18.2', '@rjsf/utils': '^5.18.2', "*

 * *                   "'@rjsf/validator-ajv8': '^5.18.2', 'antd': '^5.16.2', 'zustand': '^4.5.2'}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -9,15 +9,21 @@
     "dependencies": {
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.2.5",
         "@jupyterlab/logconsole": "^4.1.5",
         "@jupyterlab/notebook": "^4.1.5",
         "@lumino/widgets": "^2.3.1",
         "@msgpack/msgpack": "3.0.0-beta2",
-        "remeda": "^1.55.0"
+        "@rjsf/antd": "^5.18.2",
+        "@rjsf/core": "^5.18.2",
+        "@rjsf/utils": "^5.18.2",
+        "@rjsf/validator-ajv8": "^5.18.2",
+        "antd": "^5.16.2",
+        "remeda": "^1.55.0",
+        "zustand": "^4.5.2"
     },
     "description": "A JupyterLab extension. Integrate JupyterLab and Neovim",
     "devDependencies": {
         "@commitlint/cli": "^18.6.1",
         "@commitlint/config-conventional": "^18.6.3",
         "@jupyterlab/builder": "^4.1.5",
         "@jupyterlab/completer": "^4.1.5",
@@ -135,12 +141,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1",
+    "version": "0.2.2",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `neopyter-0.2.1/neopyter/labextension/static/330.aa97145ed71c9fb187d2.js` & `neopyter-0.2.2/neopyter/labextension/static/330.502c5d98d7f9486eb06c.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
     [330], {
-        330: e => {
-            e.exports = JSON.parse('{"name":"neopyter","version":"0.2.1","description":"A JupyterLab extension. Integrate JupyterLab and Neovim","workspaces":["ui-tests"],"keywords":["jupyter","jupyterlab","jupyterlab-extension","neovim"],"homepage":"https://github.com/SUSTech-data/neopyter","bugs":{"url":"https://github.com/SUSTech-data/neopyter/issues"},"license":"BSD-3-Clause","author":{"name":"Abao Zhang","email":"abaodoit@gmail.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/SUSTech-data/neopyter"},"scripts":{"build":"pnpm build:lib && pnpm build:labextension:dev","build:prod":"run-s clean build:lib:prod build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:lib:prod":"tsc","clean":"pnpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf neopyter/labextension neopyter/_version.py","clean:all":"pnpm clean:lib && pnpm clean:labextension && pnpm clean:lintcache","eslint":"pnpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"pnpm build","lint":"pnpm stylelint && pnpm prettier && pnpm eslint","lint:check":"pnpm stylelint:check && pnpm prettier:check && pnpm eslint:check","prettier":"pnpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"pnpm prettier:base --check","stylelint":"pnpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w --strict false --sourceMap","watch:labextension":"jupyter labextension watch .","prepare":"husky install"},"dependencies":{"@jupyterlab/application":"^4.1.5","@jupyterlab/apputils":"^4.2.5","@jupyterlab/logconsole":"^4.1.5","@jupyterlab/notebook":"^4.1.5","@lumino/widgets":"^2.3.1","@msgpack/msgpack":"3.0.0-beta2","remeda":"^1.55.0"},"devDependencies":{"@commitlint/cli":"^18.6.1","@commitlint/config-conventional":"^18.6.3","@jupyterlab/builder":"^4.1.5","@jupyterlab/completer":"^4.1.5","@jupyterlab/coreutils":"^6.1.5","@jupyterlab/docmanager":"^4.1.5","@jupyterlab/services":"^7.1.5","@jupyterlab/settingregistry":"^4.1.5","@jupyterlab/testutils":"^4.1.5","@jupyterlab/ui-components":"^4.1.5","@lumino/coreutils":"^2.1.2","@lumino/disposable":"^2.1.2","@types/jest":"^29.5.12","@types/json-schema":"^7.0.15","@typescript-eslint/eslint-plugin":"^6.21.0","@typescript-eslint/parser":"^6.21.0","css-loader":"^6.10.0","eslint":"^8.57.0","eslint-config-prettier":"^8.10.0","eslint-plugin-prettier":"^5.1.3","husky":"^8.0.3","jest":"^29.7.0","npm-run-all":"^4.1.5","prettier":"^3.2.5","rimraf":"^5.0.5","source-map-loader":"^1.1.3","style-loader":"^3.3.4","stylelint":"^15.11.0","stylelint-config-recommended":"^13.0.0","stylelint-config-standard":"^34.0.0","stylelint-prettier":"^4.1.0","typescript":"~5.0.4","yjs":"^13.6.14"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"neopyter/labextension"},"prettier":{"singleQuote":true,"trailingComma":"none","arrowParens":"avoid","endOfLine":"auto","overrides":[{"files":"package.json","options":{"tabWidth":4}}]},"stylelint":{"extends":["stylelint-config-recommended","stylelint-config-standard","stylelint-prettier/recommended"],"rules":{"property-no-vendor-prefix":null,"selector-no-vendor-prefix":null,"value-no-vendor-prefix":null}}}')
+        8330: e => {
+            e.exports = JSON.parse('{"name":"neopyter","version":"0.2.2","description":"A JupyterLab extension. Integrate JupyterLab and Neovim","workspaces":["ui-tests"],"keywords":["jupyter","jupyterlab","jupyterlab-extension","neovim"],"homepage":"https://github.com/SUSTech-data/neopyter","bugs":{"url":"https://github.com/SUSTech-data/neopyter/issues"},"license":"BSD-3-Clause","author":{"name":"Abao Zhang","email":"abaodoit@gmail.com"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","schema/*.json"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/SUSTech-data/neopyter"},"scripts":{"build":"pnpm build:lib && pnpm build:labextension:dev","build:prod":"run-s clean build:lib:prod build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:lib:prod":"tsc","clean":"pnpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf neopyter/labextension neopyter/_version.py","clean:all":"pnpm clean:lib && pnpm clean:labextension && pnpm clean:lintcache","eslint":"pnpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"pnpm build","lint":"pnpm stylelint && pnpm prettier && pnpm eslint","lint:check":"pnpm stylelint:check && pnpm prettier:check && pnpm eslint:check","prettier":"pnpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"pnpm prettier:base --check","stylelint":"pnpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w --strict false --sourceMap","watch:labextension":"jupyter labextension watch .","prepare":"husky install"},"dependencies":{"@jupyterlab/application":"^4.1.5","@jupyterlab/apputils":"^4.2.5","@jupyterlab/logconsole":"^4.1.5","@jupyterlab/notebook":"^4.1.5","@lumino/widgets":"^2.3.1","@msgpack/msgpack":"3.0.0-beta2","@rjsf/antd":"^5.18.2","@rjsf/core":"^5.18.2","@rjsf/utils":"^5.18.2","@rjsf/validator-ajv8":"^5.18.2","antd":"^5.16.2","remeda":"^1.55.0","zustand":"^4.5.2"},"devDependencies":{"@commitlint/cli":"^18.6.1","@commitlint/config-conventional":"^18.6.3","@jupyterlab/builder":"^4.1.5","@jupyterlab/completer":"^4.1.5","@jupyterlab/coreutils":"^6.1.5","@jupyterlab/docmanager":"^4.1.5","@jupyterlab/services":"^7.1.5","@jupyterlab/settingregistry":"^4.1.5","@jupyterlab/testutils":"^4.1.5","@jupyterlab/ui-components":"^4.1.5","@lumino/coreutils":"^2.1.2","@lumino/disposable":"^2.1.2","@types/jest":"^29.5.12","@types/json-schema":"^7.0.15","@typescript-eslint/eslint-plugin":"^6.21.0","@typescript-eslint/parser":"^6.21.0","css-loader":"^6.10.0","eslint":"^8.57.0","eslint-config-prettier":"^8.10.0","eslint-plugin-prettier":"^5.1.3","husky":"^8.0.3","jest":"^29.7.0","npm-run-all":"^4.1.5","prettier":"^3.2.5","rimraf":"^5.0.5","source-map-loader":"^1.1.3","style-loader":"^3.3.4","stylelint":"^15.11.0","stylelint-config-recommended":"^13.0.0","stylelint-config-standard":"^34.0.0","stylelint-prettier":"^4.1.0","typescript":"~5.0.4","yjs":"^13.6.14"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"schemaDir":"schema","outputDir":"neopyter/labextension"},"prettier":{"singleQuote":true,"trailingComma":"none","arrowParens":"avoid","endOfLine":"auto","overrides":[{"files":"package.json","options":{"tabWidth":4}}]},"stylelint":{"extends":["stylelint-config-recommended","stylelint-config-standard","stylelint-prettier/recommended"],"rules":{"property-no-vendor-prefix":null,"selector-no-vendor-prefix":null,"value-no-vendor-prefix":null}}}')
         }
     }
 ]);
```

### Comparing `neopyter-0.2.1/neopyter/labextension/static/537.62c041ec63a28b9c91aa.js` & `neopyter-0.2.2/neopyter/labextension/static/537.802da0d3fc85242e2b5b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
     [537], {
-        537: (n, r, t) => {
+        4537: (n, r, t) => {
             t.r(r), t.d(r, {
                 _setPath: () => Ce,
                 add: () => o,
                 addProp: () => a,
                 allPass: () => s,
                 anyPass: () => y,
                 ceil: () => g,
```

### Comparing `neopyter-0.2.1/neopyter/labextension/static/7.8eb9a8e937e5deb3af13.js` & `neopyter-0.2.2/neopyter/labextension/static/7.ff6c4288ceb2d2054177.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
     [7], {
-        7: (t, e, i) => {
+        3007: (t, e, i) => {
             i.r(e), i.d(e, {
                 DataViewIndexOutOfBoundsError: () => P,
                 DecodeError: () => u,
                 Decoder: () => W,
                 EXT_TIMESTAMP: () => d,
                 Encoder: () => I,
                 ExtData: () => h,
```

### Comparing `neopyter-0.2.1/neopyter/labextension/static/728.d85cbe66bc2da24c7357.js` & `neopyter-0.2.2/neopyter/labextension/static/728.4d0c9af16f4fa2e12590.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunkneopyter = self.webpackChunkneopyter || []).push([
     [728], {
-        475: (e, t, n) => {
+        8475: (e, t, n) => {
             n.d(t, {
                 A: () => c
             });
-            var r = n(601),
+            var r = n(1601),
                 o = n.n(r),
-                a = n(314),
+                a = n(6314),
                 s = n.n(a)()(o());
             s.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
             const c = s
         },
-        314: e => {
+        6314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = "",
                             r = void 0 !== t[5];
                         return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), r && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), r && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
@@ -34,20 +34,20 @@
                     for (var u = 0; u < e.length; u++) {
                         var p = [].concat(e[u]);
                         r && s[p[0]] || (void 0 !== a && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = a), n && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = n) : p[2] = n), o && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = o) : p[4] = "".concat(o)), t.push(p))
                     }
                 }, t
             }
         },
-        601: e => {
+        1601: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
-        72: e => {
+        5072: e => {
             var t = [];
 
             function n(e) {
                 for (var n = -1, r = 0; r < t.length; r++)
                     if (t[r].identifier === e) {
                         n = r;
                         break
@@ -105,15 +105,15 @@
                         var p = n(a[u]);
                         0 === t[p].references && (t[p].updater(), t.splice(p, 1))
                     }
                     a = i
                 }
             }
         },
-        659: e => {
+        7659: e => {
             var t = {};
             e.exports = function(e, n) {
                 var r = function(e) {
                     if (void 0 === t[e]) {
                         var n = document.querySelector(e);
                         if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                             n = n.contentDocument.head
@@ -130,21 +130,21 @@
         },
         540: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
         },
-        56: (e, t, n) => {
+        5056: (e, t, n) => {
             e.exports = function(e) {
                 var t = n.nc;
                 t && e.setAttribute("nonce", t)
             }
         },
-        825: e => {
+        7825: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
@@ -163,36 +163,36 @@
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
                     }
                 }
             }
         },
-        113: e => {
+        1113: e => {
             e.exports = function(e, t) {
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        728: (e, t, n) => {
+        9728: (e, t, n) => {
             n.r(t);
-            var r = n(72),
+            var r = n(5072),
                 o = n.n(r),
-                a = n(825),
+                a = n(7825),
                 s = n.n(a),
-                c = n(659),
+                c = n(7659),
                 i = n.n(c),
-                u = n(56),
+                u = n(5056),
                 p = n.n(u),
                 l = n(540),
                 f = n.n(l),
-                d = n(113),
+                d = n(1113),
                 v = n.n(d),
-                h = n(475),
+                h = n(8475),
                 m = {};
             m.styleTagTransform = v(), m.setAttributes = p(), m.insert = i().bind(null, "head"), m.domAPI = s(), m.insertStyleElement = f(), o()(h.A, m), h.A && h.A.locals && h.A.locals
         }
     }
 ]);
```

### Comparing `neopyter-0.2.1/neopyter/tests/server/test_handlers.py` & `neopyter-0.2.2/neopyter/tests/server/test_handlers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import asyncio
 from tornado.websocket import WebSocketClientConnection
 from neopyter.msgpack_queue import clear_queue, labextension_queue
+from neopyter.handler import settings
 import base64
 
 
-
 async def test_call_push(jp_ws_fetch):
+    settings["mode"] = "proxy"
     await clear_queue()
 
     connection: WebSocketClientConnection = await jp_ws_fetch("neopyter", "channel")
     assert isinstance(connection, WebSocketClientConnection)
     await connection.write_message(base64.standard_b64encode("Hello".encode()))
     await asyncio.sleep(1)
     assert labextension_queue.qsize() == 1
+
+    settings["mode"] = "direct"
```

### Comparing `neopyter-0.2.1/plugin/neopyter.lua` & `neopyter-0.2.2/plugin/neopyter.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/schema/labplugin.json` & `neopyter-0.2.2/schema/labplugin.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7604166666666666%*

 * *Differences: {"'definitions'": "{'mode': {'type': 'string'}}",*

 * * "'dependencies'": "OrderedDict([('mode', OrderedDict([('oneOf', [OrderedDict([('properties', "*

 * *                   "OrderedDict([('mode', OrderedDict([('enum', ['direct'])]))]))]), "*

 * *                   "OrderedDict([('properties', OrderedDict([('mode', OrderedDict([('enum', "*

 * *                   "['proxy'])])), ('ip', OrderedDict([('title', 'IP'), ('description', 'For "*

 * *                   "`proxy` mode, this is the IP of the host where jupyter server is locat […]*

```diff
@@ -1,42 +1,66 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema",
-    "additionalProperties": false,
     "definitions": {
         "ip": {
             "type": "string"
         },
         "mode": {
             "enum": [
                 "proxy",
                 "direct"
-            ]
+            ],
+            "type": "string"
         },
         "port": {
             "type": "number"
         }
     },
+    "dependencies": {
+        "mode": {
+            "oneOf": [
+                {
+                    "properties": {
+                        "mode": {
+                            "enum": [
+                                "direct"
+                            ]
+                        }
+                    }
+                },
+                {
+                    "properties": {
+                        "ip": {
+                            "$ref": "#/definitions/ip",
+                            "default": "127.0.0.1",
+                            "description": "For `proxy` mode, this is the IP of the host where jupyter server is located",
+                            "title": "IP"
+                        },
+                        "mode": {
+                            "enum": [
+                                "proxy"
+                            ]
+                        },
+                        "port": {
+                            "$ref": "#/definitions/port",
+                            "default": 9001,
+                            "title": "Port"
+                        }
+                    }
+                }
+            ]
+        }
+    },
     "description": "A JupyterLab extension. Integrate JupyterLab and Neovim",
     "jupyter.lab.setting-icon": "ui-components:neopyter",
     "jupyter.lab.setting-icon-label": "Neopyter",
     "properties": {
-        "ip": {
-            "$ref": "#/definitions/ip",
-            "default": "127.0.0.1",
-            "description": "For `proxy` mode, this is the IP of the host where jupyter server is located; For `direct` mode, this is the IP of the host where nvim is located ",
-            "title": "IP"
-        },
         "mode": {
             "$ref": "#/definitions/mode",
             "default": "direct",
-            "description": "Different work mode determine different methods of communication arcitecture. The `proxy` mode will communicate through jupyter server, while the `direct` mode will communicate directly with nvim",
-            "title": "Neopyter work mode"
-        },
-        "port": {
-            "$ref": "#/definitions/port",
-            "default": 9001,
-            "title": "Port"
+            "description": "Different work mode determine different methods of communication. The `proxy` mode will communicate through jupyter server, while the `direct` mode will communicate directly with nvim",
+            "title": "Neopyter mode"
         }
     },
     "title": "Neopyter",
     "type": "object"
 }
```

### Comparing `neopyter-0.2.1/scripts/minimal_init.lua` & `neopyter-0.2.2/scripts/minimal_init.lua`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/index.ts` & `neopyter-0.2.2/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import * as R from 'remeda';
 
 import { RpcServer, Dispatcher } from './rpcServer';
 import { WebsocketTransport } from './transport';
 import { StatusSidePanel } from './statusidepanel';
 import { statusPageIcon } from './icons';
 import { WindowedList } from '@jupyterlab/ui-components';
-import { IConfig } from './settings';
 import { DockPanel } from '@lumino/widgets';
+import { settingStore } from './store';
 
 function triggerFocus(element: HTMLElement) {
   const eventType = 'onfocusin' in element ? 'focusin' : 'focus';
   const bubbles = 'onfocusin' in element;
   let event;
 
   if ('createEvent' in document) {
@@ -58,20 +58,20 @@
     labShell: ILabShell,
     docmanager: IDocumentManager,
     nbtracker: INotebookTracker,
     restorer: ILayoutRestorer,
     settingRegistry: ISettingRegistry,
     _completionProviderManager: ICompletionProviderManager
   ) => {
+    settingStore.setSettingRegistry(settingRegistry);
     const completionProviderManager = _completionProviderManager as CompletionProviderManager;
     const providers = completionProviderManager.getProviders();
     console.log('JupyterLab extension neopyter is activated!');
     console.log('provider', completionProviderManager.getProviders());
     const kernelCompleterProvider = providers.get('CompletionProvider:kernel') as KernelCompleterProvider;
-    // completionProviderManager.updateCompleter
 
     const sidebar = new StatusSidePanel(settingRegistry);
     sidebar.title.caption = 'Neopyter';
     sidebar.title.icon = statusPageIcon;
     app.shell.add(sidebar, 'right');
 
     if (restorer) {
@@ -375,23 +375,25 @@
 
     Object.assign(dispatcher, docmanagerDispatcher);
     Object.assign(dispatcher, notebookDispatcher);
     Object.assign(dispatcher, cellDispatcher);
 
     const startConnection = async () => {
       const server = new RpcServer(dispatcher);
-
-      const { mode, ip, port } = (await settingRegistry.load('neopyter:labplugin')).composite as unknown as IConfig;
-      let url;
+      const mode = await settingStore.getMode();
+      console.log(`mode:${mode}`);
       if (mode === 'proxy') {
         const settings = ServerConnection.makeSettings();
-        url = URLExt.join(settings.wsUrl, 'neopyter', 'channel');
+        const url = URLExt.join(settings.wsUrl, 'neopyter', 'channel');
         server.start(WebsocketTransport, url, false);
       } else {
-        url = `ws://${ip}:${port}`;
+        const ip = await settingStore.getIp();
+        const port = await settingStore.getPort();
+        const url = `ws://${ip}:${port}`;
+        console.log(url);
         server.start(WebsocketTransport, url, true);
       }
     };
     startConnection();
   }
 };
```

### Comparing `neopyter-0.2.1/src/msgpackRpcProtocol.ts` & `neopyter-0.2.2/src/msgpackRpcProtocol.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/rpcServer.ts` & `neopyter-0.2.2/src/rpcServer.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/__tests__/neojupy.spec.ts` & `neopyter-0.2.2/src/__tests__/neojupy.spec.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/dispatcher/docmanager.ts` & `neopyter-0.2.2/src/dispatcher/docmanager.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/transport/base.ts` & `neopyter-0.2.2/src/transport/base.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/transport/reverseHttpTransport.ts` & `neopyter-0.2.2/src/transport/reverseHttpTransport.ts`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/src/transport/websocketTransport.ts` & `neopyter-0.2.2/src/transport/websocketTransport.ts`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
   protected onOpen(_event: Event) {
     console.log(`Connection to neopyter jupyter server by websocket ${this.websocket!.url}`);
   }
   protected onError(event: Event) {
     console.error('Websocket error', event);
   }
   protected onClose(_event: Event) {
-    console.log(`Disconnect to neopyter jupyter server by websocket ${this.websocket!.url}`);
+    console.log(`Disconnect to neopyter jupyter server by websocket ${this.websocket!.url}`, event);
     this.websocket!.close();
     this.websocket = undefined;
     this.readableStream = undefined;
     this.checkRetry();
   }
 
   protected checkRetry() {
```

### Comparing `neopyter-0.2.1/style/icons/statuspage.svg` & `neopyter-0.2.2/style/icons/statuspage.svg`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/.gitignore` & `neopyter-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/LICENSE` & `neopyter-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/README.md` & `neopyter-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,28 @@
 | <img alt="Completion" src="./doc/completion.png"> | <img alt="Cell Magic" src="./doc/cell_magic.png"> | <img alt="Line Magic" src="./doc/line_magic.png"> |
 
 ## Requirements
 
 - 📔JupyterLab >= 4.0.0
 - ✌️ Neovim nightly
   - 👍`nvim-lua/plenary.nvim`
-  - 🤏`AbaoFromCUG/websocket.nvim` (optional for `mode="proxy"`)
+  - 🤏`AbaoFromCUG/websocket.nvim` (optional for `mode="direct"`)
 
 ## Installation
 
 ### JupyterLab Extension
 
 To install the jupyterlab extension, execute:
 
 ```bash
 pip install neopyter
 ```
 
-Configure `JupyterLab` in menu `Settings`>`Settings Editor`>`Neopyter`
+Configure `JupyterLab` in side panel
+![side panel](./doc/sidepanel.png)
 
 - `mode`: refer to the previous introduction about mode
 - `IP`: if `mode=proxy`, set to the IP of the host where jupyter is located. If `proxy=direct`, set to the IP of the
   host where neovim is located
 - `port`: idle port
 
 ### Neovim plugin
```

### Comparing `neopyter-0.2.1/pyproject.toml` & `neopyter-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neopyter-0.2.1/PKG-INFO` & `neopyter-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: neopyter
-Version: 0.2.1
+Version: 0.2.2
 Dynamic: Keywords
 Summary: A JupyterLab extension. Integrate JupyterLab and Neovim
 Project-URL: Homepage, https://github.com/SUSTech-data/neopyter
 Project-URL: Bug Tracker, https://github.com/SUSTech-data/neopyter/issues
 Project-URL: Repository, https://github.com/SUSTech-data/neopyter
 Author-email: Abao Zhang <abaodoit@gmail.com>
 License: BSD 3-Clause License
@@ -94,27 +94,28 @@
 | <img alt="Completion" src="./doc/completion.png"> | <img alt="Cell Magic" src="./doc/cell_magic.png"> | <img alt="Line Magic" src="./doc/line_magic.png"> |
 
 ## Requirements
 
 - 📔JupyterLab >= 4.0.0
 - ✌️ Neovim nightly
   - 👍`nvim-lua/plenary.nvim`
-  - 🤏`AbaoFromCUG/websocket.nvim` (optional for `mode="proxy"`)
+  - 🤏`AbaoFromCUG/websocket.nvim` (optional for `mode="direct"`)
 
 ## Installation
 
 ### JupyterLab Extension
 
 To install the jupyterlab extension, execute:
 
 ```bash
 pip install neopyter
 ```
 
-Configure `JupyterLab` in menu `Settings`>`Settings Editor`>`Neopyter`
+Configure `JupyterLab` in side panel
+![side panel](./doc/sidepanel.png)
 
 - `mode`: refer to the previous introduction about mode
 - `IP`: if `mode=proxy`, set to the IP of the host where jupyter is located. If `proxy=direct`, set to the IP of the
   host where neovim is located
 - `port`: idle port
 
 ### Neovim plugin
```

