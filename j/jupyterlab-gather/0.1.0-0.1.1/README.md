# Comparing `tmp/jupyterlab_gather-0.1.0.tar.gz` & `tmp/jupyterlab_gather-0.1.1.tar.gz`

## Comparing `jupyterlab_gather-0.1.0.tar` & `jupyterlab_gather-0.1.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/babel.config.js
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/environment-dev.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jest.config.js
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/setup.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/tsconfig.test.json
--rw-r--r--   0        0        0   418752 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/yarn.lock
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/usage.md
--rw-r--r--   0        0        0   271773 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/1_landing.png
--rw-r--r--   0        0        0   120380 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/2_login.png
--rw-r--r--   0        0        0   150287 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/3_usecase.png
--rw-r--r--   0        0        0   161276 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/4_role.png
--rw-r--r--   0        0        0   168580 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/5_dashboard.png
--rw-r--r--   0        0        0   168519 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/6_roomcode.png
--rw-r--r--   0        0        0    84694 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/7_jupyter.png
--rw-r--r--   0        0        0    51633 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/8_gather.png
--rw-r--r--   0        0        0   375510 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/usage/1_preview.png
--rw-r--r--   0        0        0   289590 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/usage/2_device_options.png
--rw-r--r--   0        0        0   228510 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/usage/3_conference.png
--rw-r--r--   0        0        0   379193 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/usage/4_ar_duck.png
--rw-r--r--   0        0        0   392506 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/usage/5_model_options.png
--rw-r--r--   0        0        0   348944 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/docs/images/usage/6_run_away.png
--rw-r--r--   0        0        0   214959 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/examples/ArchDetail.FCStd
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/icons/ar.svg
--rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/icons/duckduck.svg
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/_version.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/package.json
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/schemas/jupyterlab_gather/package.json.orig
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/schemas/jupyterlab_gather/plugin.json
--rw-r--r--   0        0        0    68739 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/233.f3bbf1e2a1baf439e5b1.js
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/403.ab4b808319a194f387a7.js
--rw-r--r--   0        0        0   443982 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/469.63a09f0ed09323cb5014.js
--rw-r--r--   0        0        0    34908 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/525.d66e85209c4dd520c4e2.js
--rw-r--r--   0        0        0   616735 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/541.8a75cdffe8d6c6941693.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/541.8a75cdffe8d6c6941693.js.LICENSE.txt
--rw-r--r--   0        0        0    62494 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/554.28044d93d4fa431e2afb.js
--rw-r--r--   0        0        0    25420 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/669.beb4eb7205bbec26c381.js
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/669.beb4eb7205bbec26c381.js.LICENSE.txt
--rw-r--r--   0        0        0  1662430 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/682.983af5b493be6cf402d9.js
--rw-r--r--   0        0        0   938743 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/693.bc3659d196147d2b4d5c.js
--rw-r--r--   0        0        0    12564 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/728.bac1101ec58e0b5d9cb0.js
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/784.f33ed33b7dc0bf9c4b3f.js
--rw-r--r--   0        0        0   681134 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/964.46c0ac03c832e79889cb.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/964.46c0ac03c832e79889cb.js.LICENSE.txt
--rw-r--r--   0        0        0    46939 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/988.96f000f6347ca352a189.js
--rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/remoteEntry.0bb6bd05f11f4e9c9efa.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/style.js
--rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pattern-files/pattern-letterJ.patt
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pattern-files/pattern-letterK.patt
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pattern-files/pattern-letterL.patt
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pattern-files/pattern-letterM.patt
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pattern-files/pattern-letterN.patt
--rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pattern-files/pattern-letterP.patt
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/schema/plugin.json
--rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/arCube.ts
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/arCubePlugin.ts
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/handler.ts
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/hms.ts
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/index.ts
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/registry.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/svg.d.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/__tests__/jupyterlab_arpresent.spec.ts
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/Avatar.tsx
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/ControlBar.tsx
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/DeviceSettings.tsx
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/Icons.tsx
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/MainDisplay.tsx
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/ModelListItem.tsx
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/Peer.tsx
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/PeerSidePane.tsx
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/PresenterTile.tsx
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/Video.tsx
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/buttons/PluginButton.tsx
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/buttons/RaiseHandButton.tsx
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/buttons/ScreenShareButton.tsx
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/buttons/SettingsButton.tsx
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/modals/AddNewModelModal.tsx
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/modals/DeviceSettingModal.tsx
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/components/modals/Modal.tsx
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/layouts/GridView.tsx
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/layouts/JoinFormView.tsx
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/layouts/PresenterView.tsx
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/layouts/PreviewView.tsx
--rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/widgets/LeftSidebar.tsx
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/widgets/RightSidebar.tsx
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/src/widgets/RootDisplay.tsx
--rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/ui-tests/tests/jupyterlab_gather.spec.ts
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/LICENSE
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/README.md
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/.copier-answers.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/babel.config.js
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/environment-dev.yml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jest.config.js
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/setup.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/tsconfig.test.json
+-rw-r--r--   0        0        0   418752 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/yarn.lock
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/usage.md
+-rw-r--r--   0        0        0   271773 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/1_landing.png
+-rw-r--r--   0        0        0   120380 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/2_login.png
+-rw-r--r--   0        0        0   150287 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/3_usecase.png
+-rw-r--r--   0        0        0   161276 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/4_role.png
+-rw-r--r--   0        0        0   168580 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/5_dashboard.png
+-rw-r--r--   0        0        0   168519 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/6_roomcode.png
+-rw-r--r--   0        0        0    84694 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/7_jupyter.png
+-rw-r--r--   0        0        0    51633 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/8_gather.png
+-rw-r--r--   0        0        0   375510 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/usage/1_preview.png
+-rw-r--r--   0        0        0   289590 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/usage/2_device_options.png
+-rw-r--r--   0        0        0   228510 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/usage/3_conference.png
+-rw-r--r--   0        0        0   379193 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/usage/4_ar_duck.png
+-rw-r--r--   0        0        0   392506 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/usage/5_model_options.png
+-rw-r--r--   0        0        0   348944 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/docs/images/usage/6_run_away.png
+-rw-r--r--   0        0        0   214959 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/examples/ArchDetail.FCStd
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/icons/ar.svg
+-rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/icons/duckduck.svg
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/_version.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/package.json
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/schemas/jupyterlab_gather/package.json.orig
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/schemas/jupyterlab_gather/plugin.json
+-rw-r--r--   0        0        0    68739 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/233.f3bbf1e2a1baf439e5b1.js
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/403.ab4b808319a194f387a7.js
+-rw-r--r--   0        0        0   443982 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/469.63a09f0ed09323cb5014.js
+-rw-r--r--   0        0        0    34908 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/525.d66e85209c4dd520c4e2.js
+-rw-r--r--   0        0        0   616735 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/541.8a75cdffe8d6c6941693.js
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/541.8a75cdffe8d6c6941693.js.LICENSE.txt
+-rw-r--r--   0        0        0    62494 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/554.28044d93d4fa431e2afb.js
+-rw-r--r--   0        0        0    25420 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/669.beb4eb7205bbec26c381.js
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/669.beb4eb7205bbec26c381.js.LICENSE.txt
+-rw-r--r--   0        0        0   938743 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/693.bc3659d196147d2b4d5c.js
+-rw-r--r--   0        0        0    12564 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/728.bac1101ec58e0b5d9cb0.js
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/784.f33ed33b7dc0bf9c4b3f.js
+-rw-r--r--   0        0        0  1664008 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/92.5e78f2e47b4ce5b2a02a.js
+-rw-r--r--   0        0        0   681134 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/964.46c0ac03c832e79889cb.js
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/964.46c0ac03c832e79889cb.js.LICENSE.txt
+-rw-r--r--   0        0        0    46236 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/988.1707dba329be4f192115.js
+-rw-r--r--   0        0        0    10001 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/remoteEntry.57f38cbd174f44d793fb.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/style.js
+-rw-r--r--   0        0        0    49099 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pattern-files/pattern-letterJ.patt
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pattern-files/pattern-letterK.patt
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pattern-files/pattern-letterL.patt
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pattern-files/pattern-letterM.patt
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pattern-files/pattern-letterN.patt
+-rw-r--r--   0        0        0    12291 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pattern-files/pattern-letterP.patt
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/schema/plugin.json
+-rw-r--r--   0        0        0    17927 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/arCube.ts
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/arCubePlugin.ts
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/handler.ts
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/hms.ts
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/index.ts
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/registry.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/svg.d.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/__tests__/jupyterlab_arpresent.spec.ts
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/Avatar.tsx
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/ControlBar.tsx
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/DeviceSettings.tsx
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/Icons.tsx
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/MainDisplay.tsx
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/ModelListItem.tsx
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/Peer.tsx
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/PeerSidePane.tsx
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/PresenterTile.tsx
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/Video.tsx
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/buttons/PluginButton.tsx
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/buttons/RaiseHandButton.tsx
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/buttons/ScreenShareButton.tsx
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/buttons/SettingsButton.tsx
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/modals/AddNewModelModal.tsx
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/modals/DeviceSettingModal.tsx
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/components/modals/Modal.tsx
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/layouts/GridView.tsx
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/layouts/JoinFormView.tsx
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/layouts/PresenterView.tsx
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/layouts/PreviewView.tsx
+-rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/widgets/LeftSidebar.tsx
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/widgets/RightSidebar.tsx
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/src/widgets/RootDisplay.tsx
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/ui-tests/README.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/ui-tests/tests/jupyterlab_gather.spec.ts
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/README.md
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 jupyterlab_gather-0.1.1/PKG-INFO
```

### Comparing `jupyterlab_gather-0.1.0/.copier-answers.yml` & `jupyterlab_gather-0.1.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/RELEASE.md` & `jupyterlab_gather-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jest.config.js` & `jupyterlab_gather-0.1.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/package.json` & `jupyterlab_gather-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -221,9 +221,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_gather-0.1.0/tsconfig.json` & `jupyterlab_gather-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/yarn.lock` & `jupyterlab_gather-0.1.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/usage.md` & `jupyterlab_gather-0.1.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/1_landing.png` & `jupyterlab_gather-0.1.1/docs/images/1_landing.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/2_login.png` & `jupyterlab_gather-0.1.1/docs/images/2_login.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/3_usecase.png` & `jupyterlab_gather-0.1.1/docs/images/3_usecase.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/4_role.png` & `jupyterlab_gather-0.1.1/docs/images/4_role.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/5_dashboard.png` & `jupyterlab_gather-0.1.1/docs/images/5_dashboard.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/6_roomcode.png` & `jupyterlab_gather-0.1.1/docs/images/6_roomcode.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/7_jupyter.png` & `jupyterlab_gather-0.1.1/docs/images/7_jupyter.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/8_gather.png` & `jupyterlab_gather-0.1.1/docs/images/8_gather.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/usage/1_preview.png` & `jupyterlab_gather-0.1.1/docs/images/usage/1_preview.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/usage/2_device_options.png` & `jupyterlab_gather-0.1.1/docs/images/usage/2_device_options.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/usage/3_conference.png` & `jupyterlab_gather-0.1.1/docs/images/usage/3_conference.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/usage/4_ar_duck.png` & `jupyterlab_gather-0.1.1/docs/images/usage/4_ar_duck.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/usage/5_model_options.png` & `jupyterlab_gather-0.1.1/docs/images/usage/5_model_options.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/docs/images/usage/6_run_away.png` & `jupyterlab_gather-0.1.1/docs/images/usage/6_run_away.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/examples/ArchDetail.FCStd` & `jupyterlab_gather-0.1.1/examples/ArchDetail.FCStd`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/icons/ar.svg` & `jupyterlab_gather-0.1.1/icons/ar.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/icons/duckduck.svg` & `jupyterlab_gather-0.1.1/icons/duckduck.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/__init__.py` & `jupyterlab_gather-0.1.1/jupyterlab_gather/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/package.json` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.57f38cbd174f44d793fb.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -129,15 +129,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/QuantStack/jupyterlab-gather",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.0bb6bd05f11f4e9c9efa.js",
+            "load": "static/remoteEntry.57f38cbd174f44d793fb.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_gather"
                 },
@@ -226,9 +226,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/schemas/jupyterlab_gather/package.json.orig` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/schemas/jupyterlab_gather/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -221,9 +221,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/233.f3bbf1e2a1baf439e5b1.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/233.f3bbf1e2a1baf439e5b1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/403.ab4b808319a194f387a7.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/403.ab4b808319a194f387a7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/469.63a09f0ed09323cb5014.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/469.63a09f0ed09323cb5014.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/525.d66e85209c4dd520c4e2.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/525.d66e85209c4dd520c4e2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/541.8a75cdffe8d6c6941693.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/541.8a75cdffe8d6c6941693.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/554.28044d93d4fa431e2afb.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/554.28044d93d4fa431e2afb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/669.beb4eb7205bbec26c381.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/669.beb4eb7205bbec26c381.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/682.983af5b493be6cf402d9.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/92.5e78f2e47b4ce5b2a02a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 (self.webpackChunkjupyterlab_gather = self.webpackChunkjupyterlab_gather || []).push([
-    [682], {
+    [92], {
         4949: function(A, I, g) {
             var B, C = g(5606);
             B = A => (() => {
                 var I = {
                         799: function(A, I, g) {
                             var B;
                             "undefined" != typeof self && self, B = () => (() => {
@@ -6976,14 +6976,67 @@
                 if (I.styleSheet) I.styleSheet.cssText = A;
                 else {
                     for (; I.firstChild;) I.removeChild(I.firstChild);
                     I.appendChild(document.createTextNode(A))
                 }
             }
         },
+        869: (A, I, g) => {
+            "use strict";
+            g.d(I, {
+                j: () => E
+            });
+            var B = g(6652);
+            const C = new B.Vector3;
+
+            function Q(A, I, g, B, Q, E) {
+                const i = 2 * Math.PI * Q / 4,
+                    o = Math.max(E - 2 * Q, 0),
+                    a = Math.PI / 4;
+                C.copy(I), C[B] = 0, C.normalize();
+                const D = .5 * i / (i + o),
+                    t = 1 - C.angleTo(A) / a;
+                return 1 === Math.sign(C[g]) ? t * D : o / (i + o) + D + D * (1 - t)
+            }
+            class E extends B.BoxGeometry {
+                constructor(A = 1, I = 1, g = 1, C = 2, E = .1) {
+                    if (C = 2 * C + 1, E = Math.min(A / 2, I / 2, g / 2, E), super(1, 1, 1, C, C, C), 1 === C) return;
+                    const i = this.toNonIndexed();
+                    this.index = null, this.attributes.position = i.attributes.position, this.attributes.normal = i.attributes.normal, this.attributes.uv = i.attributes.uv;
+                    const o = new B.Vector3,
+                        a = new B.Vector3,
+                        D = new B.Vector3(A, I, g).divideScalar(2).subScalar(E),
+                        t = this.attributes.position.array,
+                        s = this.attributes.normal.array,
+                        e = this.attributes.uv.array,
+                        r = t.length / 6,
+                        w = new B.Vector3,
+                        h = .5 / C;
+                    for (let B = 0, C = 0; B < t.length; B += 3, C += 2) switch (o.fromArray(t, B), a.copy(o), a.x -= Math.sign(a.x) * h, a.y -= Math.sign(a.y) * h, a.z -= Math.sign(a.z) * h, a.normalize(), t[B + 0] = D.x * Math.sign(o.x) + a.x * E, t[B + 1] = D.y * Math.sign(o.y) + a.y * E, t[B + 2] = D.z * Math.sign(o.z) + a.z * E, s[B + 0] = a.x, s[B + 1] = a.y, s[B + 2] = a.z, Math.floor(B / r)) {
+                        case 0:
+                            w.set(1, 0, 0), e[C + 0] = Q(w, a, "z", "y", E, g), e[C + 1] = 1 - Q(w, a, "y", "z", E, I);
+                            break;
+                        case 1:
+                            w.set(-1, 0, 0), e[C + 0] = 1 - Q(w, a, "z", "y", E, g), e[C + 1] = 1 - Q(w, a, "y", "z", E, I);
+                            break;
+                        case 2:
+                            w.set(0, 1, 0), e[C + 0] = 1 - Q(w, a, "x", "z", E, A), e[C + 1] = Q(w, a, "z", "x", E, g);
+                            break;
+                        case 3:
+                            w.set(0, -1, 0), e[C + 0] = 1 - Q(w, a, "x", "z", E, A), e[C + 1] = 1 - Q(w, a, "z", "x", E, g);
+                            break;
+                        case 4:
+                            w.set(0, 0, 1), e[C + 0] = 1 - Q(w, a, "x", "y", E, A), e[C + 1] = 1 - Q(w, a, "y", "x", E, I);
+                            break;
+                        case 5:
+                            w.set(0, 0, -1), e[C + 0] = Q(w, a, "x", "y", E, A), e[C + 1] = 1 - Q(w, a, "y", "x", E, I)
+                    }
+                }
+            }
+        },
         3533: (A, I, g) => {
             "use strict";
             g.d(I, {
                 B: () => Q
             });
             var B = g(6652);
```

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/693.bc3659d196147d2b4d5c.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/693.bc3659d196147d2b4d5c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/728.bac1101ec58e0b5d9cb0.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/728.bac1101ec58e0b5d9cb0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/784.f33ed33b7dc0bf9c4b3f.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/784.f33ed33b7dc0bf9c4b3f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/964.46c0ac03c832e79889cb.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/964.46c0ac03c832e79889cb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/988.96f000f6347ca352a189.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/988.1707dba329be4f192115.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunkjupyterlab_gather = self.webpackChunkjupyterlab_gather || []).push([
     [988], {
         6641: (e, t, n) => {
             n.r(t), n.d(t, {
                 IGatherRegistryToken: () => m,
-                default: () => ie
+                default: () => re
             });
             var a = n(1201),
                 s = n(3420),
-                o = n(8107),
-                i = n(1218),
+                i = n(8107),
+                o = n(1218),
                 r = n(4814),
                 l = n(1760);
             const c = new l.LabIcon({
                     name: "jupyterlab-gather:icon_logo",
                     svgstr: '<?xml version="1.0" encoding="UTF-8" standalone="no"?>\n<svg\n   width="512"\n   height="512"\n   version="1.1"\n   viewBox="0 0 384 384"\n   id="svg106"\n   sodipodi:docname="duckduck.svg"\n   inkscape:version="1.2.2 (b0a8486541, 2022-12-01)"\n   xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape"\n   xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"\n   xmlns="http://www.w3.org/2000/svg"\n   xmlns:svg="http://www.w3.org/2000/svg">\n  <sodipodi:namedview\n     id="namedview108"\n     pagecolor="#505050"\n     bordercolor="#ffffff"\n     borderopacity="1"\n     inkscape:showpageshadow="0"\n     inkscape:pageopacity="0"\n     inkscape:pagecheckerboard="1"\n     inkscape:deskcolor="#505050"\n     showgrid="true"\n     inkscape:zoom="1.4580864"\n     inkscape:cx="293.19251"\n     inkscape:cy="208.14954"\n     inkscape:window-width="2880"\n     inkscape:window-height="1653"\n     inkscape:window-x="0"\n     inkscape:window-y="56"\n     inkscape:window-maximized="1"\n     inkscape:current-layer="svg106">\n    <inkscape:grid\n       type="xygrid"\n       id="grid1742"\n       dotted="true"\n       spacingx="7.5"\n       spacingy="7.5"\n       empcolor="#d2c538"\n       empopacity="0.83921569"\n       color="#7fa342"\n       opacity="0.14901961" />\n  </sodipodi:namedview>\n  <defs\n     id="defs26">\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2594"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2587"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2511"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:perspective\n       sodipodi:type="inkscape:persp3d"\n       inkscape:vp_x="-44.677687 : 70.826469 : 1"\n       inkscape:vp_y="0 : 683.64079 : 0"\n       inkscape:vp_z="625.53854 : 70.826469 : 1"\n       inkscape:persp3d-origin="290.43042 : 27.073459 : 1"\n       id="perspective341" />\n    <clipPath\n       id="clipPath4">\n      <rect\n         width="384"\n         height="384"\n         id="rect2" />\n    </clipPath>\n    <clipPath\n       id="clipPath8">\n      <rect\n         width="384"\n         height="384"\n         id="rect6" />\n    </clipPath>\n    <clipPath\n       id="clipPath12">\n      <rect\n         width="384"\n         height="384"\n         id="rect10" />\n    </clipPath>\n    <clipPath\n       id="clipPath16">\n      <rect\n         width="384"\n         height="384"\n         id="rect14" />\n    </clipPath>\n    <clipPath\n       id="clipPath20">\n      <rect\n         width="384"\n         height="384"\n         id="rect18" />\n    </clipPath>\n    <clipPath\n       id="clipPath24">\n      <rect\n         width="384"\n         height="384"\n         id="rect22" />\n    </clipPath>\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2511-3"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2594-3"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2511-3-5"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2511-3-9"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2511-3-6"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2511-3-62"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2594-2"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2594-23"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n    <inkscape:path-effect\n       effect="bspline"\n       id="path-effect2594-5"\n       is_visible="true"\n       lpeversion="1"\n       weight="33.333333"\n       steps="2"\n       helper_size="0"\n       apply_no_weight="true"\n       apply_with_weight="true"\n       only_selected="false" />\n  </defs>\n  <g\n     inkscape:groupmode="layer"\n     id="layer1"\n     inkscape:label="water"\n     style="display:inline" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer8"\n     inkscape:label="duck" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer3"\n     inkscape:label="duckBody"\n     style="display:inline" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer4"\n     inkscape:label="duckLeftWing"\n     style="display:inline" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer5"\n     inkscape:label="duckRightWing" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer2"\n     inkscape:label="duckHead"\n     style="fill:#ffd631;fill-opacity:1" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer6"\n     inkscape:label="duckBeak" />\n  <g\n     inkscape:groupmode="layer"\n     id="layer7"\n     inkscape:label="duckEye" />\n  <g\n     id="g3440"\n     transform="translate(2.99995,-16.741492)">\n    <path\n       style="display:inline;fill:#2eeeff;fill-opacity:1;stroke:#1b98ae;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 9.00005,111.24148 v 225 l 150,-75 v -225 l -150,75"\n       id="path2328" />\n    <path\n       style="display:inline;fill:#20c9db;fill-opacity:1;stroke:#20aec3;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 159.00005,261.24148 210,45 v -225 l -210,-45 v 225"\n       id="path2330"\n       sodipodi:nodetypes="ccccc" />\n    <path\n       style="display:inline;fill:#009bb3;fill-opacity:1;stroke:#126d85;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 9.00005,336.24148 210,45 150,-75 -210,-45 -150,75"\n       id="path2332"\n       sodipodi:nodetypes="ccccc" />\n    <path\n       id="path2442-6"\n       style="display:inline;fill:#ffb943;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 181.50005,171.24148 a 123.75,78.75 0 0 0 -123.75,78.75 123.75,78.75 0 0 0 123.75,78.75 123.75,78.75 0 0 0 123.75,-78.75 123.75,78.75 0 0 0 -0.39844,-6.2959 c 3.71787,-21.18852 5.18003,-40.34448 -3.97705,-49.92187 -8.66762,-9.06547 -26.8456,-9.5528 -47.44922,-7.85303 a 123.75,78.75 0 0 0 -71.92529,-14.6792 z" />\n    <path\n       id="path2442-6-2"\n       style="display:inline;fill:#fb9200;fill-opacity:1;stroke:none;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 63.48931,226.64334 a 123.75,78.75 0 0 0 -5.73926,23.34814 123.75,78.75 0 0 0 123.75,78.75 123.75,78.75 0 0 0 123.03809,-70.67871 123.75,78.75 0 0 1 -118.01075,55.40332 123.75,78.75 0 0 1 -123.75,-78.75 123.75,78.75 0 0 1 0.71192,-8.07275 z" />\n    <path\n       id="path2442-6-0"\n       style="display:inline;fill:none;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 181.50005,171.24148 a 123.75,78.75 0 0 0 -123.75,78.75 123.75,78.75 0 0 0 123.75,78.75 123.75,78.75 0 0 0 123.75,-78.75 123.75,78.75 0 0 0 -0.39844,-6.2959 c 3.71787,-21.18852 5.18003,-40.34448 -3.97705,-49.92187 -8.66762,-9.06547 -26.8456,-9.5528 -47.44922,-7.85303 a 123.75,78.75 0 0 0 -71.92529,-14.6792 z" />\n    <path\n       style="display:inline;fill:#ffb943;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 222.75018,203.74104 c 19.99996,-22.49995 39.99996,-44.99995 48.74993,-41.24934 8.74996,3.75062 6.25001,33.75002 -6e-5,53.74978 -6.25007,19.99976 -16.24987,29.99956 -26.24987,39.99956"\n       id="path2509"\n       inkscape:path-effect="#path-effect2511-3"\n       inkscape:original-d="m 222.75018,203.74104 c 20.00075,-22.49925 40.00075,-44.99925 60,-67.5 -2.4993,30.00135 -4.99925,60.00075 -7.5,90 -9.99945,10.00095 -19.99925,20.00075 -30,30" />\n    <path\n       id="path2509-3"\n       style="display:inline;fill:#fb9200;fill-opacity:1;stroke:none;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 275.2163,182.06104 c -1.16258,6.97806 -2.79543,13.93413 -4.7622,20.06689 C 263.194,224.76623 251.61574,236.17987 240,247.5 l 3.33984,7.79297 c 9.99999,-9.99999 19.99994,-19.99928 26.25,-39.99902 3.15213,-10.08659 5.34413,-22.70937 5.62646,-33.23291 z" />\n    <path\n       style="display:inline;fill:none;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 222.75018,203.74104 c 19.99996,-22.49995 39.99996,-44.99995 48.74993,-41.24934 8.74996,3.75062 6.25001,33.75002 -6e-5,53.74978 -6.25007,19.99976 -16.24987,29.99956 -26.24987,39.99956"\n       id="path2509-0"\n       inkscape:path-effect="#path-effect2511-3-6"\n       inkscape:original-d="m 222.75018,203.74104 c 20.00075,-22.49925 40.00075,-44.99925 60,-67.5 -2.4993,30.00135 -4.99925,60.00075 -7.5,90 -9.99945,10.00095 -19.99925,20.00075 -30,30" />\n    <ellipse\n       style="fill:#ffb943;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       id="path2387"\n       cx="132.78143"\n       cy="173.38272"\n       rx="63.75"\n       ry="60" />\n    <path\n       id="path2387-1"\n       style="fill:#fb9200;fill-opacity:1;stroke:none;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 69.847354,182.49404 a 63.75,60 0 0 0 62.934076,50.88867 63.75,60 0 0 0 62.93408,-50.88867 71.25,67.5 0 0 1 -62.93408,35.88867 71.25,67.5 0 0 1 -62.934076,-35.88867 z" />\n    <ellipse\n       style="fill:none;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       id="path2387-7"\n       cx="132.78143"\n       cy="173.38272"\n       rx="63.75"\n       ry="60" />\n    <path\n       style="fill:#ff7080;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 83.646319,167.32763 c 5.903416,-2.86002 11.127279,-7.22724 15.453442,-6.46901 4.326159,0.75822 7.753739,6.64086 11.181669,12.52409 15.26394,6.19638 30.52675,12.3923 28.03672,18.11905 -2.49003,5.72675 -22.73208,10.98424 -47.694921,9.25175 -24.962846,-1.73249 -54.645191,-10.45491 -59.95035,-16.22697 -5.305159,-5.77206 12.932616,-8.46988 26.709781,-10.728 13.777164,-2.25812 20.360242,-3.61089 26.263659,-6.47091 z"\n       id="path2592"\n       inkscape:path-effect="#path-effect2594"\n       inkscape:original-d="m 84.32576,168.83492 c 5.22441,-4.36679 10.44827,-8.73401 15.67189,-13.1019 3.42828,5.88382 10.28378,17.64969 10.28378,17.64969 15.26378,6.19676 30.52659,12.39269 45.78938,18.58814 -20.24253,5.25829 -40.48457,10.51579 -60.72737,15.7728 -29.683186,-8.72219 -59.365533,-17.4446 -89.048813,-26.16778 19.073184,-2.82077 37.002612,-7.60308 57.217365,-8.46388 8.080918,0.53598 14.447518,-1.87025 20.813768,-4.27707 z"\n       sodipodi:nodetypes="czcccccc" />\n    <path\n       id="path2592-7"\n       style="fill:#f9005a;fill-opacity:0.828653;stroke:none;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 31.442794,179.73198 c -1.67491,1.20871 -2.08707,2.60472 -0.57129,4.25391 5.30516,5.77206 34.98737,14.49505 59.950196,16.22754 24.96282,1.73249 45.20528,-3.52521 47.69531,-9.25195 0.62544,-1.43843 0.12773,-2.9058 -1.20556,-4.396 -9.28186,4.6367 -27.61372,7.79812 -48.93604,6.20361 -20.144896,-1.50645 -42.917586,-7.25686 -56.932616,-13.03711 z" />\n    <path\n       style="fill:none;fill-opacity:1;stroke:#480400;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 83.646319,167.32763 c 5.903416,-2.86002 11.127279,-7.22724 15.453442,-6.46901 4.326159,0.75822 7.753739,6.64086 11.181669,12.52409 15.26394,6.19638 30.52675,12.3923 28.03672,18.11905 -2.49003,5.72675 -22.73208,10.98424 -47.694922,9.25175 -24.962847,-1.73249 -54.645191,-10.45491 -59.950348,-16.22697 -5.305156,-5.77206 12.932611,-8.46988 26.709778,-10.728 13.777166,-2.25812 20.360244,-3.61089 26.263661,-6.47091 z"\n       id="path2592-9"\n       inkscape:path-effect="#path-effect2594-5"\n       inkscape:original-d="m 84.32576,168.83492 c 5.22441,-4.36679 10.44827,-8.73401 15.67189,-13.1019 3.42828,5.88382 10.28378,17.64969 10.28378,17.64969 15.26378,6.19676 30.52659,12.39269 45.78938,18.58814 -20.24253,5.25829 -40.48457,10.51579 -60.72737,15.7728 -29.683188,-8.72219 -59.365535,-17.4446 -89.048815,-26.16778 19.07319,-2.82077 37.00261,-7.60308 57.217367,-8.46388 8.080918,0.53598 14.447518,-1.87025 20.813768,-4.27707 z"\n       sodipodi:nodetypes="czcccccc" />\n    <ellipse\n       style="fill:#fb9200;fill-opacity:1;stroke:none;stroke-width:4.20001;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       id="path2684-9"\n       cx="156.99413"\n       cy="175.19801"\n       rx="11.849189"\n       ry="11.433258" />\n    <ellipse\n       style="fill:#2f0300;fill-opacity:1;stroke:none;stroke-width:4.20001;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       id="path2684"\n       cx="156.67303"\n       cy="173.78844"\n       rx="11.25"\n       ry="9.8404236" />\n    <circle\n       style="fill:#fbc892;fill-opacity:0.464482;stroke:none;stroke-width:4.2;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       id="path2686"\n       cx="160.08458"\n       cy="170.52603"\n       r="3.75" />\n    <path\n       id="path1752"\n       style="display:inline;fill:none;fill-opacity:1;stroke:#08415c;stroke-width:9;stroke-linecap:round;stroke-linejoin:round;stroke-dasharray:none;stroke-opacity:1"\n       d="m 219.00005,156.24148 150,-75 m -360,30 150,-75 210,45 v 225 l -150,75 m -210,-270 v 225 l 210,45 v -225 l -210,-45"\n       inkscape:label="cubeFrame"\n       sodipodi:nodetypes="cccccccccccc" />\n  </g>\n</svg>\n'
                 }),
                 d = new l.LabIcon({
@@ -54,26 +54,26 @@
             const E = ({
                     children: e,
                     title: t,
                     isOpen: n,
                     hasCloseBtn: a,
                     onClose: s
                 }) => {
-                    const [o, i] = (0, k.useState)(n), r = (0, k.useRef)(null);
+                    const [i, o] = (0, k.useState)(n), r = (0, k.useRef)(null);
                     (0, k.useEffect)((() => {
-                        i(n)
+                        o(n)
                     }), [n]), (0, k.useEffect)((() => {
                         const e = r.current;
-                        e && (o ? (e.showModal(), e.addEventListener("mousedown", l)) : (e.removeEventListener("mousedown", l), e.close()))
-                    }), [o]);
+                        e && (i ? (e.showModal(), e.addEventListener("mousedown", l)) : (e.removeEventListener("mousedown", l), e.close()))
+                    }), [i]);
                     const l = e => {
                             e.target === e.currentTarget && c()
                         },
                         c = () => {
-                            s && s(), i(!1)
+                            s && s(), o(!1)
                         };
                     return w().createElement("dialog", {
                         ref: r,
                         onKeyDown: e => {
                             "Escape" === e.key && c()
                         },
                         className: "jlab-gather-modal"
@@ -95,108 +95,108 @@
                 }) => {
                     const a = (0, k.useRef)(null),
                         s = (0, S.uniqueNamesGenerator)({
                             dictionaries: [S.adjectives, S.animals],
                             style: "capital",
                             separator: " "
                         }),
-                        [o, i] = (0, k.useState)({
+                        [i, o] = (0, k.useState)({
                             name: s,
                             url: ""
                         });
                     (0, k.useEffect)((() => {
                         t && a.current && setTimeout((() => {
                             a.current.focus()
                         }), 0)
                     }), [t]);
                     const r = e => {
                         const {
                             name: t,
                             value: n
                         } = e.target;
-                        i((e => ({
+                        o((e => ({
                             ...e,
                             [t]: n
                         })))
                     };
                     return w().createElement(E, {
                         title: "Add a New Model",
                         hasCloseBtn: !0,
                         isOpen: t,
                         onClose: n
                     }, w().createElement("form", {
                         className: "jlab-gather-form",
                         onSubmit: t => {
-                            t.preventDefault(), e(o), i({
+                            t.preventDefault(), e(i), o({
                                 name: s,
                                 url: ""
                             })
                         }
                     }, w().createElement("div", {
                         className: "jlab-gather-form-input"
                     }, w().createElement("label", {
                         htmlFor: "userName"
                     }, "Model Name"), w().createElement("input", {
                         required: !0,
                         className: "jlab-gather-input",
                         name: "name",
                         type: "text",
                         placeholder: "Model Name",
-                        value: o.name,
+                        value: i.name,
                         onChange: r
                     })), w().createElement("div", {
                         className: "jlab-gather-form-input"
                     }, w().createElement("label", {
                         htmlFor: "room-code"
                     }, "Model Url"), w().createElement("input", {
                         required: !0,
                         className: "jlab-gather-input",
                         name: "url",
                         type: "text",
                         placeholder: "Model Url",
-                        value: o.url,
+                        value: i.url,
                         onChange: r
                     })), w().createElement("button", {
                         className: "jlab-gather-btn-common jlab-gather-btn-primary"
                     }, "Add Model")))
                 };
             var C = n(6469);
-            const M = new C.JC,
-                N = g.HMSRoomProvider,
-                _ = M.getStore(),
-                A = M.getActions();
+            const N = new C.JC,
+                M = g.HMSRoomProvider,
+                _ = N.getStore(),
+                A = N.getActions();
             A.initAppData({
                 canLoadModel: !0,
                 modelRegistry: [],
                 isPresenting: !1,
                 presenterId: "",
                 selectedModel: null,
                 loadedModels: [],
                 isConnecting: !1
             }), A.setLogLevel(C.JZ.WARN);
-            const I = ({
+            const x = ({
                 modelList: e,
                 modelRegistry: t
             }) => {
-                const [n, a] = (0, k.useState)(!1), [s, o] = (0, k.useState)(!1), [i, r] = (0, k.useState)(void 0), [c, d] = (0, k.useState)(), [p, h] = (0, k.useState)(!1);
+                const [n, a] = (0, k.useState)(!1), [s, i] = (0, k.useState)(!1), [o, r] = (0, k.useState)(void 0), [c, d] = (0, k.useState)(), [p, h] = (0, k.useState)(!1);
                 (0, k.useEffect)((() => {
                     r(_.getState((0, g.selectAppData)("arCube"))), _.subscribe(u, (0, g.selectAppData)("canLoadModel")), _.subscribe(m, (0, g.selectAppData)("arCube"))
                 }), []);
                 const m = () => {
                         r(_.getState((0, g.selectAppData)("arCube")))
                     },
                     u = () => {
                         const e = _.getState((0, g.selectAppData)("canLoadModel"));
                         a(!e)
                     },
                     f = e => {
                         d(e), A.setAppData("selectedModel", e)
                     },
                     S = e => {
-                        i || r(_.getState((0, g.selectAppData)("arCube"))), c ? null == i || i.changeModelInScene(e, c.name) : console.log("Model must be selected")
+                        o || r(_.getState((0, g.selectAppData)("arCube"))), c ? null == o || o.changeModelInScene(e, c.name) : console.log("Model must be selected")
                     },
                     E = () => {
                         h(!1)
                     };
                 return w().createElement("div", {
                     className: "jlab-gather-sidebar-container"
                 }, w().createElement("div", {
@@ -231,34 +231,34 @@
                     onSubmit: e => {
                         t.registerModel(e), E()
                     },
                     onClose: E
                 }), w().createElement(l.Button, {
                     className: "jlab-gather-sidebar-load-button",
                     onClick: () => {
-                        s ? null == i || i.disableSecondScene() : null == i || i.enableSecondScene(), o(!s)
+                        s ? null == o || o.disableSecondScene() : null == o || o.enableSecondScene(), i(!s)
                     },
                     disabled: n
                 }, n ? w().createElement(y.FontAwesomeIcon, {
                     icon: b.faSpinner,
                     className: "jlab-gather-spinner"
                 }) : s ? "Disable Second Model" : "Load Second Model")))
             };
-            class x extends l.SidePanel {
+            class I extends l.SidePanel {
                 constructor(e) {
                     super({
                         content: new f.Panel
                     }), this._signal = e.modelRegistryChanged, this.addClass("jlab-gather-sidebar-widget"), this.title.icon = d, this.title.className, this.title.caption = "Augmented reality";
                     const t = document.createElement("h2");
                     t.textContent = "augmented reality", this.header.addWidget(new f.Widget({
                         node: t
                     }));
                     const n = s.ReactWidget.create(w().createElement(l.UseSignal, {
                         signal: this._signal
-                    }, (() => w().createElement(I, {
+                    }, (() => w().createElement(x, {
                         modelList: this._modelList,
                         modelRegistry: e
                     }))));
                     this.content.addWidget(n), this._signal.connect(((e, t) => {
                         this._modelList = this.addModelToRegistryArray(t), this.updateModel(t.name)
                     }))
                 }
@@ -271,48 +271,48 @@
                 updateModel(e) {
                     const t = _.getState((0, g.selectAppData)("loadedModels")),
                         n = _.getState((0, g.selectAppData)("arCube")),
                         a = t.findIndex((t => t === e));
                     n && -1 !== a && n.changeModelInScene(a, t[a])
                 }
             }
-            var P = n(2037),
-                D = n.n(P);
+            var D = n(2037),
+                P = n.n(D);
             n(4796);
             const T = ({
                     sceneNumber: e,
                     initialScale: t,
                     arCube: n
                 }) => {
                     const [a, s] = (0, k.useState)(t);
                     return w().createElement("div", {
                         className: "jlab-gather-scale-slider"
-                    }, w().createElement("p", null, 0 === e ? "First Model" : "Second Model"), w().createElement(D(), {
+                    }, w().createElement("p", null, 0 === e ? "First Model" : "Second Model"), w().createElement(P(), {
                         className: "slider",
                         min: t / 4,
                         max: 4 * t,
                         defaultValue: t,
                         value: a,
                         step: .001,
                         onChange: t => ((e, t) => {
                             n && (n.setScale(e, t), s(e))
                         })(t, e)
                     }))
                 },
                 R = () => {
-                    const [e, t] = (0, k.useState)(void 0), [n, a] = (0, k.useState)(!1), [s, o] = (0, k.useState)(1), [i, r] = (0, k.useState)(1);
+                    const [e, t] = (0, k.useState)(void 0), [n, a] = (0, k.useState)(!1), [s, i] = (0, k.useState)(1), [o, r] = (0, k.useState)(1);
                     (0, k.useEffect)((() => {
                         t(_.getState((0, g.selectAppData)("arCube"))), _.subscribe(l, (0, g.selectAppData)("arCube"))
                     }), []);
                     const l = () => {
                             const e = _.getState((0, g.selectAppData)("arCube"));
                             e && (e.secondSceneSignal.connect(d), e.scaleSignal.connect(c), t(e))
                         },
                         c = (e, t) => {
-                            0 === t.sceneNumber ? o(t.scale) : r(t.scale)
+                            0 === t.sceneNumber ? i(t.scale) : r(t.scale)
                         },
                         d = (e, t) => {
                             a(t)
                         };
                     return w().createElement("div", {
                         className: "jlab-gather-sidebar-container"
                     }, w().createElement("div", {
@@ -321,32 +321,32 @@
                         className: "jlab-gather-sidebar-list jlab-gather-sidebar-right"
                     }, w().createElement(T, {
                         sceneNumber: 0,
                         initialScale: s,
                         arCube: e
                     }), n ? w().createElement(T, {
                         sceneNumber: 1,
-                        initialScale: i,
+                        initialScale: o,
                         arCube: e
                     }) : null))
                 };
-            class V extends l.SidePanel {
+            class L extends l.SidePanel {
                 constructor() {
                     super({
                         content: new f.Panel
                     }), this.addClass("jlab-gather-sidebar-widget"), this.title.icon = d, this.title.className, this.title.caption = "Augmented reality";
                     const e = document.createElement("h2");
                     e.textContent = "augmented reality", this.header.addWidget(new f.Widget({
                         node: e
                     }));
                     const t = s.ReactWidget.create(w().createElement(R, null));
                     this.content.addWidget(t)
                 }
             }
-            const L = ({
+            const B = ({
                     children: e
                 }) => w().createElement("div", {
                     className: "jlab-gather-avatar"
                 }, e),
                 F = ({
                     peer: e,
                     className: t
@@ -365,126 +365,126 @@
                         ref: n,
                         className: `jlab-gather-peer-video jlab-gather-peer-video-${t} \n            ${e.isHandRaised?"jlab-gather-peer-hand-raised":""}\n            ${e.isLocal?"jlab-gather-local":""}`,
                         autoPlay: !0,
                         muted: !0,
                         playsInline: !0
                     }), w().createElement("div", {
                         className: "jlab-gather-peer-name"
-                    }, e.name)) : w().createElement(L, null, (e => {
+                    }, e.name)) : w().createElement(B, null, (e => {
                         const t = e.split(/[_-\s]+/).map((e => e.charAt(0)));
                         return t ? null == t ? void 0 : t.join("") : "Woops"
                     })(e.name)))
                 },
-                B = () => {
+                z = () => {
                     const e = (0, g.useHMSStore)(g.selectPeers);
                     return w().createElement("div", {
                         className: "jlab-gather-main-grid-container"
                     }, w().createElement("div", {
                         className: "jlab-gather-main-grid-view"
                     }, e.map((e => w().createElement(F, {
                         key: e.id,
                         peer: e,
                         className: "grid"
                     })))))
                 },
-                z = ({
+                H = ({
                     state: e
                 }) => {
                     const t = (0, g.useHMSActions)(),
                         [n, a] = (0, k.useState)(""),
                         s = (0, S.uniqueNamesGenerator)({
                             dictionaries: [S.adjectives, S.colors, S.animals],
                             style: "capital",
                             separator: " "
                         }),
-                        [o, i] = (0, k.useState)({
+                        [i, o] = (0, k.useState)({
                             userName: s,
                             roomCode: n
                         });
                     (0, k.useEffect)((() => {
                         (async () => {
                             try {
                                 const t = await e.fetch("jupyterlab_gather");
                                 if (t) {
                                     const e = t.roomCode;
-                                    i({
+                                    o({
                                         userName: s,
                                         roomCode: e
                                     }), a(e)
                                 }
                             } catch (e) {
                                 console.log("Error fetching room code", e)
                             }
                         })()
                     }), []);
                     const r = e => {
-                        i((t => ({
+                        o((t => ({
                             ...t,
                             [e.target.name]: e.target.value
                         })))
                     };
                     return w().createElement("form", {
                         className: "jlab-gather-form",
                         onSubmit: async n => {
                             n.preventDefault(), console.log("clicking join"), t.setAppData("isConnecting", !0);
                             const {
                                 userName: a = "",
                                 roomCode: s = ""
-                            } = o;
+                            } = i;
                             await e.save("jupyterlab_gather", {
                                 roomCode: s
                             });
-                            const i = {
+                            const o = {
                                 userName: a,
                                 authToken: await t.getAuthTokenByRoomCode({
                                     roomCode: s
                                 }),
                                 settings: {
                                     isAudioMuted: !0,
                                     isVideoMuted: !1
                                 },
                                 metaData: ""
                             };
-                            t.setAppData("config", i);
+                            t.setAppData("config", o);
                             try {
                                 await t.preview({
-                                    ...i
+                                    ...o
                                 })
                             } catch (n) {
                                 console.error(n)
                             }
                         }
                     }, w().createElement("h2", null, "Join Room"), w().createElement("div", {
                         className: "jlab-gather-form-input"
                     }, w().createElement("label", {
                         htmlFor: "userName"
                     }, "Username"), w().createElement("input", {
                         required: !0,
                         className: "jlab-gather-input",
-                        value: o.userName,
+                        value: i.userName,
                         onChange: r,
                         type: "text",
                         name: "userName",
                         placeholder: "Your name"
                     })), w().createElement("div", {
                         className: "jlab-gather-form-input"
                     }, w().createElement("label", {
                         htmlFor: "room-code"
                     }, "Room ID"), w().createElement("input", {
                         type: "text",
                         className: "jlab-gather-input",
                         name: "roomCode",
                         placeholder: "Room code",
                         onChange: r,
-                        value: o.roomCode
+                        value: i.roomCode
                     })), w().createElement("button", {
                         className: "jlab-gather-btn-common jlab-gather-btn-primary"
                     }, "Join"))
                 },
-                H = ({
+                V = ({
                     peers: e
                 }) => w().createElement("div", {
                     className: "jlab-gather-peer-sidepane-list"
                 }, e.map((e => w().createElement(F, {
                     key: e.id,
                     peer: e,
                     className: "sidepane"
@@ -519,15 +519,15 @@
                     }), []), w().createElement("div", {
                         className: "jlab-gather-presenter-container-main"
                     }, w().createElement("div", {
                         className: "jlab-gather-presenter-container"
                     }, t ? w().createElement(w().Fragment, null, w().createElement(G, {
                         peer: t,
                         className: "jlab-gather-presenter-video"
-                    })) : w().createElement("div", null, "Waiting...")), w().createElement(H, {
+                    })) : w().createElement("div", null, "Waiting...")), w().createElement(V, {
                         peers: e.filter((e => e.id !== (null == t ? void 0 : t.id)))
                     }))
                 },
                 O = ({
                     trackId: e,
                     className: t
                 }) => {
@@ -570,16 +570,16 @@
                 }) => {
                     const n = (0, k.useRef)(null),
                         {
                             allDevices: a,
                             updateDevice: s
                         } = (0, g.useDevices)(),
                         {
-                            videoInput: o,
-                            audioInput: i,
+                            videoInput: i,
+                            audioInput: o,
                             audioOutput: r
                         } = a;
                     (0, k.useEffect)((() => {
                         e && n.current && setTimeout((() => {
                             n.current.focus()
                         }), 0)
                     }), [e]);
@@ -594,19 +594,19 @@
                         hasCloseBtn: !0,
                         isOpen: e,
                         onClose: t
                     }, w().createElement("div", {
                         className: "jlab-gather-device-settings-container"
                     }, w().createElement(U, {
                         title: "Camera",
-                        list: o,
+                        list: i,
                         onChange: e => l(e.target.value, g.DeviceType.videoInput)
                     }), w().createElement(U, {
                         title: "Microphone",
-                        list: i,
+                        list: o,
                         onChange: e => l(e.target.value, g.DeviceType.audioInput)
                     }), w().createElement(U, {
                         title: "Speaker",
                         list: r,
                         onChange: e => l(e.target.value, g.DeviceType.audioOutput)
                     })))
                 },
@@ -660,36 +660,37 @@
                         onClick: () => {
                             e.setAppData("isConnecting", !1)
                         }
                     }, "Back"), w().createElement($, null))))
                 };
             var K = n(4949),
                 Q = n(8881),
-                Y = n(3533);
-            const Z = class {
+                Y = n(869),
+                Z = n(3533);
+            const X = class {
                     constructor() {
                         this.onSuccessfulLoad = (e, t, n) => {
                             console.log("on successful load", e, n);
                             const a = e.scene;
                             a.name = `model${t}`, a.children.forEach((e => {
                                 const t = e.children.filter((e => !e.name.startsWith("edge-")));
                                 e.children = t
                             })), this.animations = e.animations, this.mixer = new Q.AnimationMixer(a), this.animations && this.animations.forEach((e => {
                                 this.mixer.clipAction(e).play()
                             }));
                             const s = (new Q.Box3).setFromObject(a),
-                                o = this.calcScale(this.bgCubeBoundingBox, s);
-                            a.scale.set(o, o, o);
-                            const i = (new Q.Box3).setFromObject(a),
+                                i = this.calcScale(this.bgCubeBoundingBox, s);
+                            a.scale.set(i, i, i);
+                            const o = (new Q.Box3).setFromObject(a),
                                 r = new Q.Vector3;
-                            i.getCenter(r), a.position.set(-r.x, -r.y, -r.z), this.sceneGroups[t].add(a), this.okToLoadModel = !0;
+                            o.getCenter(r), a.position.set(-r.x, -r.y, -r.z), this.sceneGroups[t].add(a), this.okToLoadModel = !0;
                             const l = [...this.loadedModels.slice(0, t), n, ...this.loadedModels.slice(t)];
                             A.setAppData("loadedModels", l), A.setAppData("canLoadModel", !0), this.scaleSignal.emit({
                                 sceneNumber: t,
-                                scale: o
+                                scale: i
                             }), console.log("model loaded parse")
                         }, this.secondSceneSignal = new h.Signal(this), this.scaleSignal = new h.Signal(this), this.bgCubeCenter = new Q.Vector3, this.initialize()
                     }
                     initialize() {
                         this.sceneGroups = [], this.loadedModels = [], _.subscribe(this.setupSource.bind(this), (0, g.selectAppData)("videoDeviceId")), this.setupThreeStuff(), this.setupSource(), this.setupContext(), this.setupMarkerRoots(), this.setupScene(0)
                     }
                     setupThreeStuff() {
@@ -717,14 +718,17 @@
                         console.log("setting up source");
                         const e = _.getState((0, g.selectAppData)("videoDeviceId"));
                         this.arToolkitSource = new K.ArToolkitSource({
                             sourceType: "webcam",
                             deviceId: e
                         }), this.arjsVid = document.getElementById("arjs-video"), this.arjsVid && this.arjsVid.remove(), this.arToolkitSource.init()
                     }
+                    getThemeColor() {
+                        return getComputedStyle(document.body).getPropertyValue("--jp-layout-color0")
+                    }
                     setupContext() {
                         console.log("setting up context"), this.arToolkitContext = new K.ArToolkitContext({
                             cameraParametersUrl: K.ArToolkitContext.baseURL + "../data/data/camera_para.dat",
                             detectionMode: "mono"
                         }), this.arToolkitContext.init((() => {
                             this.camera.projectionMatrix.copy(this.arToolkitContext.getProjectionMatrix())
                         }))
@@ -750,32 +754,24 @@
                             const a = new Q.Group;
                             this.hiroGroupArray.push(a), a.position.y = -.625, a.rotation.setFromVector3(e[t]), n.add(a)
                         }
                     }
                     setupScene(e) {
                         console.log("setting up scene");
                         const t = new Q.Group;
-                        t.scale.set(.875, .875, .875), t.name = `scene${e}`, t.add(new Q.Mesh(new Q.BoxGeometry(2, 2, 2), new Q.MeshBasicMaterial({
-                            color: "#2EEEFF",
-                            side: Q.BackSide
-                        })));
-                        const n = new Q.Group,
-                            a = new Q.CylinderGeometry(.03, .03, 2, 32),
-                            s = [new Q.Vector3(0, -1, -1), new Q.Vector3(0, 1, -1), new Q.Vector3(0, -1, 1), new Q.Vector3(0, 1, 1), new Q.Vector3(-1, 0, -1), new Q.Vector3(1, 0, -1), new Q.Vector3(-1, 0, 1), new Q.Vector3(1, 0, 1), new Q.Vector3(-1, -1, 0), new Q.Vector3(1, -1, 0), new Q.Vector3(-1, 1, 0), new Q.Vector3(1, 1, 0)],
-                            o = [new Q.Vector3(0, 0, Math.PI / 2), new Q.Vector3(0, 0, Math.PI / 2), new Q.Vector3(0, 0, Math.PI / 2), new Q.Vector3(0, 0, Math.PI / 2), new Q.Vector3(0, 0, 0), new Q.Vector3(0, 0, 0), new Q.Vector3(0, 0, 0), new Q.Vector3(0, 0, 0), new Q.Vector3(Math.PI / 2, 0, 0), new Q.Vector3(Math.PI / 2, 0, 0), new Q.Vector3(Math.PI / 2, 0, 0), new Q.Vector3(Math.PI / 2, 0, 0)];
-                        for (let e = 0; e < 12; e++) {
-                            const t = new Q.Mesh(a, new Q.MeshLambertMaterial({
-                                color: "#262626"
+                        t.scale.set(.875, .875, .875), t.name = `scene${e}`;
+                        const n = this.getThemeColor(),
+                            a = new Q.Mesh(new Y.j(2, 2, 2, 7, .1), new Q.MeshBasicMaterial({
+                                color: n,
+                                side: Q.BackSide
                             }));
-                            t.position.copy(s[e]), t.rotation.setFromVector3(o[e]), n.add(t)
-                        }
-                        n.name = "edge-group", t.add(n), this.sceneGroups.push(t), this.bgCubeBoundingBox || (this.bgCubeBoundingBox = (new Q.Box3).setFromObject(n), this.bgCubeBoundingBox.getCenter(this.bgCubeCenter)), this.loadModel(e), console.log("fin")
+                        t.add(a), this.sceneGroups.push(t), this.bgCubeBoundingBox || (this.bgCubeBoundingBox = (new Q.Box3).setFromObject(a), this.bgCubeBoundingBox.getCenter(this.bgCubeCenter)), this.loadModel(e), console.log("fin")
                     }
                     loadModel(e, t) {
-                        console.log("loading model", e, t), this.gltfLoader || (this.gltfLoader = new Y.B);
+                        console.log("loading model", e, t), this.gltfLoader || (this.gltfLoader = new Z.B);
                         const n = t || "duck",
                             a = this.findModelByName(n);
                         if (console.log("model", a), this.okToLoadModel = !1, A.setAppData("canLoadModel", !1), "url" in a) this.gltfLoader.load(a.url, (t => {
                             this.onSuccessfulLoad(t, e, n)
                         }), (() => {
                             console.log("model loading")
                         }), (e => {
@@ -790,16 +786,16 @@
                             }))
                         }
                     }
                     calcScale(e, t) {
                         const n = Math.abs(e.max.x - e.min.x),
                             a = Math.abs(e.max.y - e.min.y),
                             s = Math.abs(e.max.z - e.min.z),
-                            o = [n / Math.abs(t.max.x - t.min.x), a / Math.abs(t.max.y - t.min.y), s / Math.abs(t.max.z - t.min.z)];
-                        return Math.min(...o)
+                            i = [n / Math.abs(t.max.x - t.min.x), a / Math.abs(t.max.y - t.min.y), s / Math.abs(t.max.z - t.min.z)];
+                        return Math.min(...i)
                     }
                     findModelByName(e) {
                         return _.getState((0, g.selectAppData)("modelRegistry")).find((t => t.name === e))
                     }
                     changeModelInScene(e, t) {
                         const n = this.sceneGroups[e],
                             a = n.getObjectByName(`model${e}`);
@@ -842,246 +838,246 @@
                             for (let e = 0; e < 6; e++)
                                 if (this.hiroRootArray[e].visible) {
                                     this.hiroGroupArray[e].add(this.sceneGroups[1]);
                                     break
                                 }
                     }
                 },
-                X = class {
+                ee = class {
                     constructor() {
                         this.input = null, this.output = null
                     }
                     blendImages(e, t) {
                         if (e.width !== t.width || e.height !== t.height) throw new Error("ImageData dimensions must match");
                         const n = new ImageData(e.width, e.height);
                         for (let a = 0; a < n.data.length; a += 4) {
                             const s = t.data[a + 3] / 255,
-                                o = 1 - s;
-                            n.data[a] = e.data[a] * o + t.data[a] * s, n.data[a + 1] = e.data[a + 1] * o + t.data[a + 1] * s, n.data[a + 2] = e.data[a + 2] * o + t.data[a + 2] * s, n.data[a + 3] = 255
+                                i = 1 - s;
+                            n.data[a] = e.data[a] * i + t.data[a] * s, n.data[a + 1] = e.data[a + 1] * i + t.data[a + 1] * s, n.data[a + 2] = e.data[a + 2] * i + t.data[a + 2] * s, n.data[a + 3] = 255
                         }
                         return n
                     }
                     flipImageDataVertically(e) {
                         const t = e.width,
                             n = e.height,
                             a = new Uint8ClampedArray(t * n * 4);
                         for (let s = 0; s < n; s++)
-                            for (let o = 0; o < t; o++) {
-                                const i = 4 * (s * t + o),
-                                    r = 4 * ((n - s - 1) * t + o);
-                                a[r] = e.data[i], a[r + 1] = e.data[i + 1], a[r + 2] = e.data[i + 2], a[r + 3] = e.data[i + 3]
+                            for (let i = 0; i < t; i++) {
+                                const o = 4 * (s * t + i),
+                                    r = 4 * ((n - s - 1) * t + i);
+                                a[r] = e.data[o], a[r + 1] = e.data[o + 1], a[r + 2] = e.data[o + 2], a[r + 3] = e.data[o + 3]
                             }
                         return new ImageData(a, t, n)
                     }
                     processVideoFrame(e, t) {
                         if (!e || !t) throw new Error("Plugin invalid input/output");
                         this.input = e, this.output = t;
                         const n = e.width,
                             a = e.height;
                         t.width = n, t.height = a;
                         const s = e.getContext("2d"),
-                            o = null == s ? void 0 : s.getImageData(0, 0, n, a),
-                            i = new Uint8Array(n * a * 4);
-                        this.arCube.renderer.readRenderTargetPixels(this.arCube.renderTarget, 0, 0, n, a, i);
-                        const r = new ImageData(new Uint8ClampedArray(i), n, a),
+                            i = null == s ? void 0 : s.getImageData(0, 0, n, a),
+                            o = new Uint8Array(n * a * 4);
+                        this.arCube.renderer.readRenderTargetPixels(this.arCube.renderTarget, 0, 0, n, a, o);
+                        const r = new ImageData(new Uint8ClampedArray(o), n, a),
                             l = t.getContext("2d");
-                        o || console.log("no image input data");
+                        i || console.log("no image input data");
                         const c = this.flipImageDataVertically(r),
-                            d = this.blendImages(o, c);
+                            d = this.blendImages(i, c);
                         null == l || l.putImageData(d, 0, 0)
                     }
                     getName() {
                         return "arcube-plugin"
                     }
                     isSupported() {
                         return !0
                     }
                     checkSupport() {
                         return {
                             isSupported: !0
                         }
                     }
                     async init() {
-                        this.arCube = new Z, A.setAppData("arCube", this.arCube), this.arCube.animate()
+                        this.arCube = new X, A.setAppData("arCube", this.arCube), this.arCube.animate()
                     }
                     getPluginType() {
                         return C.Nq.TRANSFORM
                     }
                     getContextType() {
                         return C.iu["2D"]
                     }
                     stop() {
                         const e = document.getElementById("arjs-video");
                         null == e || e.remove()
                     }
                 },
-                ee = () => {
+                te = () => {
                     const e = (0, g.useHMSActions)(),
                         t = (0, g.useHMSStore)(g.selectLocalPeer),
                         n = (0, g.useHMSStore)((0, g.selectSessionStore)("isPresenting")),
                         a = (0, g.useHMSStore)((0, g.selectSessionStore)("presenterId")),
                         s = (0, g.useHMSStore)(g.selectLocalPeerRole),
-                        o = new X,
-                        i = (0, g.useHMSStore)((0, g.selectIsLocalVideoPluginPresent)(o.getName())),
+                        i = new ee,
+                        o = (0, g.useHMSStore)((0, g.selectIsLocalVideoPluginPresent)(i.getName())),
                         [r, l] = (0, k.useState)(!1),
                         [c, d] = (0, k.useState)();
                     (0, k.useEffect)((() => {
                         e.sessionStore.observe("isPresenting"), e.sessionStore.observe("presenterId"), s && d(s)
                     }), [e]), (0, k.useEffect)((() => {
                         a && (null == t ? void 0 : t.id) !== a.id ? l(!0) : l(!1)
                     }), [n, a]);
                     const p = n => {
                         t && n ? e.changeRoleOfPeer(t.id, n, !0) : console.log("Problem setting role")
                     };
                     return w().createElement("button", {
                         className: "jlab-gather-btn-control",
                         onClick: async () => {
-                            i || n ? (console.log("removing"), p(null == c ? void 0 : c.name), e.sessionStore.set("isPresenting", !1), e.sessionStore.set("presenterId", ""), await e.removePluginFromVideoTrack(o)) : (console.log("adding"), p("presenter"), e.sessionStore.set("isPresenting", !0), e.sessionStore.set("presenterId", t), await e.addPluginToVideoTrack(o))
+                            o || n ? (console.log("removing"), p(null == c ? void 0 : c.name), e.sessionStore.set("isPresenting", !1), e.sessionStore.set("presenterId", ""), await e.removePluginFromVideoTrack(i)) : (console.log("adding"), p("presenter"), e.sessionStore.set("isPresenting", !0), e.sessionStore.set("presenterId", t), await e.addPluginToVideoTrack(i))
                         },
                         disabled: r
                     }, r ? w().createElement(y.FontAwesomeIcon, {
                         icon: b.faBan,
                         className: "jlab-gather-icon"
-                    }) : n || i ? w().createElement(y.FontAwesomeIcon, {
+                    }) : n || o ? w().createElement(y.FontAwesomeIcon, {
                         icon: b.faEyeSlash,
                         className: "jlab-gather-icon"
                     }) : w().createElement(y.FontAwesomeIcon, {
                         icon: b.faEye,
                         className: "jlab-gather-icon"
                     }))
                 },
-                te = () => {
+                ne = () => {
                     const e = (0, g.useHMSStore)(g.selectLocalPeerID),
                         t = (0, g.useHMSStore)((0, g.selectHasPeerHandRaised)(e)),
                         n = (0, g.useHMSActions)(),
                         a = (0, k.useCallback)((async () => {
                             t ? await n.lowerLocalPeerHand() : await n.raiseLocalPeerHand()
                         }), [n, t]);
                     return w().createElement("button", {
                         className: "jlab-gather-btn-control",
                         onClick: a
                     }, w().createElement(y.FontAwesomeIcon, {
                         icon: b.faHand,
                         className: "jlab-gather-icon " + (t ? "jlab-gather-icon-breathe" : "")
                     }))
                 },
-                ne = () => {
+                ae = () => {
                     const e = (0, g.useHMSActions)(),
                         t = (0, g.useHMSStore)(g.selectLocalPeer),
                         n = (0, g.useHMSStore)((0, g.selectSessionStore)("presenterId")),
                         {
                             isLocalAudioEnabled: a,
                             isLocalVideoEnabled: s,
-                            toggleAudio: o,
-                            toggleVideo: i
+                            toggleAudio: i,
+                            toggleVideo: o
                         } = (0, g.useAVToggle)();
                     return (0, k.useEffect)((() => {
                         e.sessionStore.observe("presenterId")
                     }), [e]), w().createElement("div", {
                         id: "jlab-gather-control-bar",
                         className: "jlab-gather-control-bar"
                     }, w().createElement("button", {
                         className: "jlab-gather-btn-control",
-                        onClick: o
+                        onClick: i
                     }, a ? w().createElement(y.FontAwesomeIcon, {
                         icon: b.faMicrophone,
                         className: "jlab-gather-icon"
                     }) : w().createElement(y.FontAwesomeIcon, {
                         icon: b.faMicrophoneSlash,
                         className: "jlab-gather-icon"
                     })), w().createElement("button", {
                         className: "jlab-gather-btn-control",
-                        onClick: i
+                        onClick: o
                     }, s ? w().createElement(y.FontAwesomeIcon, {
                         icon: b.faVideo,
                         className: "jlab-gather-icon"
                     }) : w().createElement(y.FontAwesomeIcon, {
                         icon: b.faVideoSlash,
                         className: "jlab-gather-icon"
-                    })), w().createElement(ee, null), w().createElement(te, null), w().createElement($, null), w().createElement("button", {
+                    })), w().createElement(te, null), w().createElement(ne, null), w().createElement($, null), w().createElement("button", {
                         className: "jlab-gather-btn-control jlab-gather-btn-danger",
                         onClick: async () => {
                             (null == t ? void 0 : t.id) === (null == n ? void 0 : n.id) && (await e.sessionStore.set("isPresenting", !1), await e.sessionStore.set("presenterId", "")), e.leave()
                         }
                     }, w().createElement(y.FontAwesomeIcon, {
                         icon: b.faPersonThroughWindow,
                         className: "jlab-gather-icon"
                     })))
                 },
-                ae = ({
+                se = ({
                     state: e
                 }) => {
                     const t = (0, g.useHMSActions)(),
                         n = (0, g.useHMSStore)(g.selectIsConnectedToRoom),
                         a = (0, g.useHMSStore)((0, g.selectAppData)("isConnecting")),
                         s = (0, g.useHMSStore)((0, g.selectSessionStore)("isPresenting"));
                     return (0, k.useEffect)((() => {
                         n && t.setAppData("isConnecting", !1)
                     }), [n]), (0, k.useEffect)((() => {
                         n && (t.sessionStore.observe("isPresenting"), t.sessionStore.observe("presenterId")), window.onunload = () => {
                             n && t.leave()
                         }
-                    }), [t, n]), w().createElement(w().Fragment, null, s ? w().createElement(W, null) : n ? w().createElement(B, null) : a ? w().createElement(J, null) : w().createElement(z, {
+                    }), [t, n]), w().createElement(w().Fragment, null, s ? w().createElement(W, null) : n ? w().createElement(z, null) : a ? w().createElement(J, null) : w().createElement(H, {
                         state: e
-                    }), n && w().createElement(ne, null))
+                    }), n && w().createElement(ae, null))
                 },
-                se = ({
+                ie = ({
                     node: e,
                     modelRegistryChanged: t,
                     state: n
                 }) => {
                     const a = (0, k.useRef)(null);
                     return (0, k.useEffect)((() => {
                         if (a.current) {
                             const e = a.current.parentElement;
                             null == e || e.classList.add("jlab-gather-overflow")
                         }
                     }), [a]), w().createElement("div", {
                         ref: a,
                         className: "jlab-gather-root"
-                    }, w().createElement(ae, {
+                    }, w().createElement(se, {
                         state: n
                     }))
                 };
             class oe extends l.ReactWidget {
                 constructor(e, t) {
                     super(), this._modelRegistryChanged = e, this._state = t
                 }
                 render() {
-                    return w().createElement(N, null, w().createElement(se, {
+                    return w().createElement(M, null, w().createElement(ie, {
                         node: this.node,
                         modelRegistryChanged: this._modelRegistryChanged,
                         state: this._state
                     }))
                 }
             }
-            const ie = [{
+            const re = [{
                 id: "jupyterlab_gather",
                 description: "Video presentation over WebRTC with AR capabilities.",
                 autoStart: !0,
-                requires: [s.ICommandPalette, o.ILauncher, m, r.IStateDB],
-                optional: [a.ILayoutRestorer, i.ISettingRegistry],
-                activate: (e, t, n, a, o, i, r) => {
+                requires: [s.ICommandPalette, i.ILauncher, m, r.IStateDB],
+                optional: [a.ILayoutRestorer, o.ISettingRegistry],
+                activate: (e, t, n, a, i, o, r) => {
                     let l;
                     console.log("JupyterLab extension jupyterlab_gather is activated!");
                     const d = "gather:open";
                     e.commands.addCommand(d, {
                         label: "Start Gather",
                         icon: c,
                         execute: () => {
                             if (!l || l.isDisposed) {
-                                const e = new oe(a.modelRegistryChanged, o);
+                                const e = new oe(a.modelRegistryChanged, i);
                                 l = new s.MainAreaWidget({
                                     content: e
                                 }), l.id = "gather-jupyterlab", l.title.label = "AR Presentation", l.title.closable = !0, l.title.icon = c
                             }
                             l.isAttached || e.shell.add(l, "main");
-                            const t = new x(a);
+                            const t = new I(a);
                             t.id = "gather-leftSidePanel";
-                            const n = new V;
+                            const n = new L;
                             n.id = "gather-rightSidePanel", e.shell.activateById(l.id), e.shell.add(l, "main"), e.shell.add(t, "left", {
                                 rank: 2e3
                             }), e.shell.add(n, "right", {
                                 rank: 2e3
                             }), a.registerModel({
                                 name: "duck",
                                 url: "https://github.khronos.org/glTF-Sample-Viewer-Release/assets/models/Models/Duck/glTF/Duck.gltf"
```

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/remoteEntry.0bb6bd05f11f4e9c9efa.js` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/remoteEntry.57f38cbd174f44d793fb.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, f, i, l, u, d, s, c, h, b, p, v, m, g, y, w, j, P = {
-            4297: (e, r, t) => {
+            6558: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(469), t.e(682), t.e(345), t.e(988)]).then((() => () => t(6641))),
-                        "./extension": () => Promise.all([t.e(469), t.e(682), t.e(345), t.e(988)]).then((() => () => t(6641))),
+                        "./index": () => Promise.all([t.e(469), t.e(92), t.e(345), t.e(988)]).then((() => () => t(6641))),
+                        "./extension": () => Promise.all([t.e(469), t.e(92), t.e(345), t.e(988)]).then((() => () => t(6641))),
                         "./style": () => t.e(728).then((() => () => t(9728)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -44,46 +44,46 @@
         }), r
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
+        92: "5e78f2e47b4ce5b2a02a",
         233: "f3bbf1e2a1baf439e5b1",
         345: "26c0e249fc145531615c",
         403: "ab4b808319a194f387a7",
         469: "63a09f0ed09323cb5014",
         525: "d66e85209c4dd520c4e2",
         541: "8a75cdffe8d6c6941693",
         554: "28044d93d4fa431e2afb",
         628: "ac2ffb26a9f247fb590e",
         669: "beb4eb7205bbec26c381",
-        682: "983af5b493be6cf402d9",
         693: "bc3659d196147d2b4d5c",
         728: "bac1101ec58e0b5d9cb0",
         784: "f33ed33b7dc0bf9c4b3f",
         964: "46c0ac03c832e79889cb",
-        988: "96f000f6347ca352a189",
+        988: "1707dba329be4f192115",
         999: "7e3b509e32b7c0922298"
     } [e] + ".js?v=" + {
+        92: "5e78f2e47b4ce5b2a02a",
         233: "f3bbf1e2a1baf439e5b1",
         345: "26c0e249fc145531615c",
         403: "ab4b808319a194f387a7",
         469: "63a09f0ed09323cb5014",
         525: "d66e85209c4dd520c4e2",
         541: "8a75cdffe8d6c6941693",
         554: "28044d93d4fa431e2afb",
         628: "ac2ffb26a9f247fb590e",
         669: "beb4eb7205bbec26c381",
-        682: "983af5b493be6cf402d9",
         693: "bc3659d196147d2b4d5c",
         728: "bac1101ec58e0b5d9cb0",
         784: "f33ed33b7dc0bf9c4b3f",
         964: "46c0ac03c832e79889cb",
-        988: "96f000f6347ca352a189",
+        988: "1707dba329be4f192115",
         999: "7e3b509e32b7c0922298"
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -136,15 +136,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : f > i.from)) && (n[r] = {
                             get: t,
                             from: f,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (i("@100mslive/react-sdk", "0.10.3", (() => Promise.all([k.e(469), k.e(525), k.e(345), k.e(628)]).then((() => () => k(1525))))), i("@fortawesome/fontawesome-svg-core", "6.5.2", (() => k.e(554).then((() => () => k(6554))))), i("@fortawesome/free-solid-svg-icons", "6.5.2", (() => k.e(693).then((() => () => k(6693))))), i("@fortawesome/react-fontawesome", "0.2.2", (() => Promise.all([k.e(345), k.e(999), k.e(784)]).then((() => () => k(6784))))), i("jupyterlab_gather", "0.1.0", (() => Promise.all([k.e(469), k.e(682), k.e(345), k.e(988)]).then((() => () => k(6641))))), i("rc-slider", "10.6.2", (() => Promise.all([k.e(669), k.e(345)]).then((() => () => k(7669))))), i("three", "0.150.1", (() => k.e(541).then((() => () => k(6541))))), i("three", "0.162.0", (() => k.e(964).then((() => () => k(8964))))), i("unique-names-generator", "4.7.1", (() => k.e(233).then((() => () => k(8233)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@100mslive/react-sdk", "0.10.3", (() => Promise.all([k.e(469), k.e(525), k.e(345), k.e(628)]).then((() => () => k(1525))))), i("@fortawesome/fontawesome-svg-core", "6.5.2", (() => k.e(554).then((() => () => k(6554))))), i("@fortawesome/free-solid-svg-icons", "6.5.2", (() => k.e(693).then((() => () => k(6693))))), i("@fortawesome/react-fontawesome", "0.2.2", (() => Promise.all([k.e(345), k.e(999), k.e(784)]).then((() => () => k(6784))))), i("jupyterlab_gather", "0.1.1", (() => Promise.all([k.e(469), k.e(92), k.e(345), k.e(988)]).then((() => () => k(6641))))), i("rc-slider", "10.6.2", (() => Promise.all([k.e(669), k.e(345)]).then((() => () => k(7669))))), i("three", "0.150.1", (() => k.e(541).then((() => () => k(6541))))), i("three", "0.162.0", (() => k.e(964).then((() => () => k(8964))))), i("unique-names-generator", "4.7.1", (() => k.e(233).then((() => () => k(8233)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -332,10 +332,10 @@
                     i && i(k)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], k.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunkjupyterlab_gather = self.webpackChunkjupyterlab_gather || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), k.nc = void 0;
-    var E = k(4297);
+    var E = k(6558);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).jupyterlab_gather = E
 })();
```

### Comparing `jupyterlab_gather-0.1.0/jupyterlab_gather/labextension/static/third-party-licenses.json` & `jupyterlab_gather-0.1.1/jupyterlab_gather/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pattern-files/pattern-letterJ.patt` & `jupyterlab_gather-0.1.1/pattern-files/pattern-letterJ.patt`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pattern-files/pattern-letterK.patt` & `jupyterlab_gather-0.1.1/pattern-files/pattern-letterK.patt`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pattern-files/pattern-letterL.patt` & `jupyterlab_gather-0.1.1/pattern-files/pattern-letterL.patt`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pattern-files/pattern-letterM.patt` & `jupyterlab_gather-0.1.1/pattern-files/pattern-letterM.patt`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pattern-files/pattern-letterN.patt` & `jupyterlab_gather-0.1.1/pattern-files/pattern-letterN.patt`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pattern-files/pattern-letterP.patt` & `jupyterlab_gather-0.1.1/pattern-files/pattern-letterP.patt`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/arCube.ts` & `jupyterlab_gather-0.1.1/src/arCube.ts`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,19 @@
   selectAppData,
   selectIsSomeoneScreenSharing
 } from '@100mslive/react-sdk';
 //@ts-expect-error AR.js doesn't have type definitions
 import * as THREEx from '@ar-js-org/ar.js/three.js/build/ar-threex.js';
 import { Signal } from '@lumino/signaling';
 import * as THREE from 'three';
+import { RoundedBoxGeometry } from 'three/examples/jsm/geometries/RoundedBoxGeometry';
 import { GLTF, GLTFLoader } from 'three/examples/jsm/loaders/GLTFLoader';
 import { hmsActions, hmsStore } from './hms';
 import { IModelRegistryData } from './registry';
+
 const FIRST_SCENE = 0;
 const SECOND_SCENE = 1;
 
 export interface IScaleSignal {
   sceneNumber: number;
   scale: number;
 }
@@ -201,14 +203,21 @@
     if (this.arjsVid) {
       this.arjsVid.remove();
     }
 
     this.arToolkitSource.init();
   }
 
+  getThemeColor() {
+    const layoutColor = getComputedStyle(document.body);
+    const cubeColorValue = layoutColor.getPropertyValue('--jp-layout-color0');
+
+    return cubeColorValue;
+  }
+
   // updateSource() {
   //   const deviceId = hmsStore.getState(selectAppData('videoDeviceId'));
 
   //   this.arToolkitSource = new THREEx.ArToolkitSource({
   //     sourceType: 'webcam',
   //     deviceId
   //   });
@@ -320,80 +329,34 @@
   setupScene(sceneNumber: number) {
     console.log('setting up scene');
     const sceneGroup = new THREE.Group();
     // a 1x1x1 cube model with scale factor 1.25 fills up the physical cube
     sceneGroup.scale.set(1.75 / 2, 1.75 / 2, 1.75 / 2);
     sceneGroup.name = `scene${sceneNumber}`;
 
+    const cubeColor = this.getThemeColor();
+
     // reversed cube
     //TODO: Can probably just have one cube and add it to scenes as needed
-    sceneGroup.add(
-      new THREE.Mesh(
-        new THREE.BoxGeometry(2, 2, 2),
-        new THREE.MeshBasicMaterial({
-          color: '#2EEEFF',
-          side: THREE.BackSide
-        })
-      )
-    );
 
-    // cube edges
-    const edgeGroup = new THREE.Group();
-    const edgeGeometry = new THREE.CylinderGeometry(0.03, 0.03, 2, 32);
-
-    const edgeCenters = [
-      new THREE.Vector3(0, -1, -1),
-      new THREE.Vector3(0, 1, -1),
-      new THREE.Vector3(0, -1, 1),
-      new THREE.Vector3(0, 1, 1),
-      new THREE.Vector3(-1, 0, -1),
-      new THREE.Vector3(1, 0, -1),
-      new THREE.Vector3(-1, 0, 1),
-      new THREE.Vector3(1, 0, 1),
-      new THREE.Vector3(-1, -1, 0),
-      new THREE.Vector3(1, -1, 0),
-      new THREE.Vector3(-1, 1, 0),
-      new THREE.Vector3(1, 1, 0)
-    ];
-
-    const edgeRotations = [
-      new THREE.Vector3(0, 0, Math.PI / 2),
-      new THREE.Vector3(0, 0, Math.PI / 2),
-      new THREE.Vector3(0, 0, Math.PI / 2),
-      new THREE.Vector3(0, 0, Math.PI / 2),
-      new THREE.Vector3(0, 0, 0),
-      new THREE.Vector3(0, 0, 0),
-      new THREE.Vector3(0, 0, 0),
-      new THREE.Vector3(0, 0, 0),
-      new THREE.Vector3(Math.PI / 2, 0, 0),
-      new THREE.Vector3(Math.PI / 2, 0, 0),
-      new THREE.Vector3(Math.PI / 2, 0, 0),
-      new THREE.Vector3(Math.PI / 2, 0, 0)
-    ];
-
-    for (let i = 0; i < 12; i++) {
-      const edge = new THREE.Mesh(
-        edgeGeometry,
-        new THREE.MeshLambertMaterial({
-          color: '#262626'
-        })
-      );
-      edge.position.copy(edgeCenters[i]);
-      edge.rotation.setFromVector3(edgeRotations[i]);
+    const bgCube = new THREE.Mesh(
+      new RoundedBoxGeometry(2, 2, 2, 7, 0.1),
+      new THREE.MeshBasicMaterial({
+        color: cubeColor,
+        side: THREE.BackSide
+      })
+    );
 
-      edgeGroup.add(edge);
-    }
+    sceneGroup.add(bgCube);
 
-    edgeGroup.name = 'edge-group';
-    sceneGroup.add(edgeGroup);
     this.sceneGroups.push(sceneGroup);
 
     // Set up BG cubes bounding box and center
     if (!this.bgCubeBoundingBox) {
-      this.bgCubeBoundingBox = new THREE.Box3().setFromObject(edgeGroup);
+      this.bgCubeBoundingBox = new THREE.Box3().setFromObject(bgCube);
       this.bgCubeBoundingBox.getCenter(this.bgCubeCenter);
     }
 
     this.loadModel(sceneNumber);
     console.log('fin');
   }
```

### Comparing `jupyterlab_gather-0.1.0/src/arCubePlugin.ts` & `jupyterlab_gather-0.1.1/src/arCubePlugin.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/handler.ts` & `jupyterlab_gather-0.1.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/hms.ts` & `jupyterlab_gather-0.1.1/src/hms.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/index.ts` & `jupyterlab_gather-0.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/registry.ts` & `jupyterlab_gather-0.1.1/src/registry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/ControlBar.tsx` & `jupyterlab_gather-0.1.1/src/components/ControlBar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/DeviceSettings.tsx` & `jupyterlab_gather-0.1.1/src/components/DeviceSettings.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/MainDisplay.tsx` & `jupyterlab_gather-0.1.1/src/components/MainDisplay.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/ModelListItem.tsx` & `jupyterlab_gather-0.1.1/src/components/ModelListItem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/Peer.tsx` & `jupyterlab_gather-0.1.1/src/components/Peer.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/PresenterTile.tsx` & `jupyterlab_gather-0.1.1/src/components/PresenterTile.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/buttons/PluginButton.tsx` & `jupyterlab_gather-0.1.1/src/components/buttons/PluginButton.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/buttons/RaiseHandButton.tsx` & `jupyterlab_gather-0.1.1/src/components/buttons/RaiseHandButton.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/buttons/ScreenShareButton.tsx` & `jupyterlab_gather-0.1.1/src/components/buttons/ScreenShareButton.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/buttons/SettingsButton.tsx` & `jupyterlab_gather-0.1.1/src/components/buttons/SettingsButton.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/modals/AddNewModelModal.tsx` & `jupyterlab_gather-0.1.1/src/components/modals/AddNewModelModal.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/modals/DeviceSettingModal.tsx` & `jupyterlab_gather-0.1.1/src/components/modals/DeviceSettingModal.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/components/modals/Modal.tsx` & `jupyterlab_gather-0.1.1/src/components/modals/Modal.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/layouts/GridView.tsx` & `jupyterlab_gather-0.1.1/src/layouts/GridView.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/layouts/JoinFormView.tsx` & `jupyterlab_gather-0.1.1/src/layouts/JoinFormView.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/layouts/PresenterView.tsx` & `jupyterlab_gather-0.1.1/src/layouts/PresenterView.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/layouts/PreviewView.tsx` & `jupyterlab_gather-0.1.1/src/layouts/PreviewView.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/widgets/LeftSidebar.tsx` & `jupyterlab_gather-0.1.1/src/widgets/LeftSidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/widgets/RightSidebar.tsx` & `jupyterlab_gather-0.1.1/src/widgets/RightSidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/src/widgets/RootDisplay.tsx` & `jupyterlab_gather-0.1.1/src/widgets/RootDisplay.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/style/base.css` & `jupyterlab_gather-0.1.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/ui-tests/README.md` & `jupyterlab_gather-0.1.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/ui-tests/tests/jupyterlab_gather.spec.ts` & `jupyterlab_gather-0.1.1/ui-tests/tests/jupyterlab_gather.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/.gitignore` & `jupyterlab_gather-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/LICENSE` & `jupyterlab_gather-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/README.md` & `jupyterlab_gather-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/pyproject.toml` & `jupyterlab_gather-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_gather-0.1.0/PKG-INFO` & `jupyterlab_gather-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_gather
-Version: 0.1.0
+Version: 0.1.1
 Dynamic: Keywords
 Summary: Video presentation over WebRTC with AR capabilities.
 Project-URL: Homepage, https://github.com/QuantStack/jupyterlab-gather
 Project-URL: Bug Tracker, https://github.com/QuantStack/jupyterlab-gather/issues
 Project-URL: Repository, https://github.com/QuantStack/jupyterlab-gather.git
 Author-email: Greg Mooney <gregory.mooney@quantstack.net>
 License: BSD 3-Clause License
```

