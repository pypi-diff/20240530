# Comparing `tmp/webdiff-1.0.0.tar.gz` & `tmp/webdiff-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdiff-1.0.0.tar", last modified: Thu May 30 20:08:17 2024, max compression
+gzip compressed data, was "webdiff-1.0.1.tar", last modified: Thu May 30 20:12:34 2024, max compression
```

## Comparing `webdiff-1.0.0.tar` & `webdiff-1.0.1.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.519662 webdiff-1.0.0/
--rw-r--r--   0 danvk      (501) staff       (20)    11323 2022-09-06 14:09:42.000000 webdiff-1.0.0/LICENSE
--rw-r--r--   0 danvk      (501) staff       (20)       91 2022-09-06 14:09:42.000000 webdiff-1.0.0/MANIFEST.in
--rw-r--r--   0 danvk      (501) staff       (20)     8144 2024-05-30 20:08:17.519460 webdiff-1.0.0/PKG-INFO
--rw-r--r--   0 danvk      (501) staff       (20)     7377 2024-05-30 20:08:02.000000 webdiff-1.0.0/README.md
--rw-r--r--   0 danvk      (501) staff       (20)       38 2024-05-30 20:08:17.519716 webdiff-1.0.0/setup.cfg
--rw-r--r--   0 danvk      (501) staff       (20)     1381 2024-05-30 20:06:20.000000 webdiff-1.0.0/setup.py
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.463296 webdiff-1.0.0/webdiff/
--rw-r--r--   0 danvk      (501) staff       (20)        0 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/__init__.py
--rwxr-xr-x   0 danvk      (501) staff       (20)     9698 2024-05-30 19:28:24.000000 webdiff-1.0.0/webdiff/app.py
--rw-r--r--   0 danvk      (501) staff       (20)     3708 2024-05-30 19:50:00.000000 webdiff-1.0.0/webdiff/argparser.py
--rw-r--r--   0 danvk      (501) staff       (20)     4934 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/diff.py
--rw-r--r--   0 danvk      (501) staff       (20)     2770 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/dirdiff.py
--rw-r--r--   0 danvk      (501) staff       (20)     4439 2024-05-30 19:46:15.000000 webdiff-1.0.0/webdiff/github_fetcher.py
--rw-r--r--   0 danvk      (501) staff       (20)     2254 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/githubdiff.py
--rwxr-xr-x   0 danvk      (501) staff       (20)     1019 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/gitwebdiff.py
--rw-r--r--   0 danvk      (501) staff       (20)     1809 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/localfilediff.py
--rw-r--r--   0 danvk      (501) staff       (20)     1632 2024-05-30 15:27:35.000000 webdiff-1.0.0/webdiff/options.py
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.464151 webdiff-1.0.0/webdiff/static/
--rw-r--r--   0 danvk      (501) staff       (20)        0 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/__init__.py
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.464806 webdiff-1.0.0/webdiff/static/codediff.js/
--rw-r--r--   0 danvk      (501) staff       (20)     2807 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/codediff.js/codediff.css
--rw-r--r--   0 danvk      (501) staff       (20)    22168 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/codediff.js/codediff.js
--rwxr-xr-x   0 danvk      (501) staff       (20)    11308 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/codediff.js/difflib.js
--rw-r--r--   0 danvk      (501) staff       (20)     2162 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/codediff.js/googlecode.css
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.465375 webdiff-1.0.0/webdiff/static/css/
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.466144 webdiff-1.0.0/webdiff/static/css/Inconsolata/
--rwxr-xr-x   0 danvk      (501) staff       (20)    67724 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/css/Inconsolata/Inconsolata-Bold.ttf
--rwxr-xr-x   0 danvk      (501) staff       (20)    84868 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/css/Inconsolata/Inconsolata-Regular.ttf
--rwxr-xr-x   0 danvk      (501) staff       (20)     4498 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/css/Inconsolata/OFL.txt
--rw-r--r--   0 danvk      (501) staff       (20)     1053 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/css/googlecode.css
--rw-r--r--   0 danvk      (501) staff       (20)      189 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/css/inconsolata.css
--rw-r--r--   0 danvk      (501) staff       (20)     3239 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/style.css
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.477416 webdiff-1.0.0/webdiff/static/css/themes/
--rw-r--r--   0 danvk      (501) staff       (20)     1158 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/a11y-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1146 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/a11y-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1357 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/agate.css
--rw-r--r--   0 danvk      (501) staff       (20)      961 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/an-old-hope.css
--rw-r--r--   0 danvk      (501) staff       (20)      611 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/androidstudio.css
--rw-r--r--   0 danvk      (501) staff       (20)      844 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/arduino-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      673 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/arta.css
--rw-r--r--   0 danvk      (501) staff       (20)      454 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/ascetic.css
--rw-r--r--   0 danvk      (501) staff       (20)     1193 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/atom-one-dark-reasonable.css
--rw-r--r--   0 danvk      (501) staff       (20)      856 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/atom-one-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)      856 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/atom-one-light.css
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.502946 webdiff-1.0.0/webdiff/static/css/themes/base16/
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/3024.css
--rw-r--r--   0 danvk      (501) staff       (20)     1403 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/apathy.css
--rw-r--r--   0 danvk      (501) staff       (20)     1368 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/apprentice.css
--rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ashes.css
--rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-cave-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-cave.css
--rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-dune-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-dune.css
--rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-estuary-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-estuary.css
--rw-r--r--   0 danvk      (501) staff       (20)     1416 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-forest-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1410 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-forest.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-heath-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-heath.css
--rw-r--r--   0 danvk      (501) staff       (20)     1418 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-lakeside-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-lakeside.css
--rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-plateau-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-plateau.css
--rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-savanna-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-savanna.css
--rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-seaside-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-seaside.css
--rw-r--r--   0 danvk      (501) staff       (20)     1421 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-sulphurpool-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1415 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-sulphurpool.css
--rw-r--r--   0 danvk      (501) staff       (20)     1391 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/atlas.css
--rw-r--r--   0 danvk      (501) staff       (20)     1368 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/bespin.css
--rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-bathory.css
--rw-r--r--   0 danvk      (501) staff       (20)     1375 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-burzum.css
--rw-r--r--   0 danvk      (501) staff       (20)     1390 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-dark-funeral.css
--rw-r--r--   0 danvk      (501) staff       (20)     1387 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-gorgoroth.css
--rw-r--r--   0 danvk      (501) staff       (20)     1377 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-immortal.css
--rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-khold.css
--rw-r--r--   0 danvk      (501) staff       (20)     1384 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-marduk.css
--rw-r--r--   0 danvk      (501) staff       (20)     1384 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-mayhem.css
--rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-nile.css
--rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-venom.css
--rw-r--r--   0 danvk      (501) staff       (20)     1372 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal.css
--rw-r--r--   0 danvk      (501) staff       (20)     1404 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/brewer.css
--rw-r--r--   0 danvk      (501) staff       (20)     1396 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/bright.css
--rw-r--r--   0 danvk      (501) staff       (20)     1407 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/brogrammer.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/brush-trees-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1407 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/brush-trees.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/chalk.css
--rw-r--r--   0 danvk      (501) staff       (20)     1451 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/circus.css
--rw-r--r--   0 danvk      (501) staff       (20)     1400 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/classic-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/classic-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/codeschool.css
--rw-r--r--   0 danvk      (501) staff       (20)     1361 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/colors.css
--rw-r--r--   0 danvk      (501) staff       (20)     1400 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/cupcake.css
--rw-r--r--   0 danvk      (501) staff       (20)     1347 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/cupertino.css
--rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/danqing.css
--rw-r--r--   0 danvk      (501) staff       (20)     1367 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/darcula.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/dark-violet.css
--rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/darkmoss.css
--rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/darktooth.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/decaf.css
--rw-r--r--   0 danvk      (501) staff       (20)     1405 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/default-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/default-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/dirtysea.css
--rw-r--r--   0 danvk      (501) staff       (20)     1456 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/dracula.css
--rw-r--r--   0 danvk      (501) staff       (20)     1387 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/edge-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1388 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/edge-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1380 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/eighties.css
--rw-r--r--   0 danvk      (501) staff       (20)     1403 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/embers.css
--rw-r--r--   0 danvk      (501) staff       (20)     1382 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1381 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-gray-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-gray-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1424 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/espresso.css
--rw-r--r--   0 danvk      (501) staff       (20)     1396 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/eva-dim.css
--rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/eva.css
--rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/flat.css
--rw-r--r--   0 danvk      (501) staff       (20)     1394 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/framer.css
--rw-r--r--   0 danvk      (501) staff       (20)     1369 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/fruit-soda.css
--rw-r--r--   0 danvk      (501) staff       (20)     1404 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gigavolt.css
--rw-r--r--   0 danvk      (501) staff       (20)     1339 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/github.css
--rw-r--r--   0 danvk      (501) staff       (20)     1387 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/google-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/google-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/grayscale-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/grayscale-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1354 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/green-screen.css
--rw-r--r--   0 danvk      (501) staff       (20)     1449 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-hard.css
--rw-r--r--   0 danvk      (501) staff       (20)     1451 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-medium.css
--rw-r--r--   0 danvk      (501) staff       (20)     1449 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-pale.css
--rw-r--r--   0 danvk      (501) staff       (20)     1449 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-soft.css
--rw-r--r--   0 danvk      (501) staff       (20)     1450 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-light-hard.css
--rw-r--r--   0 danvk      (501) staff       (20)     1452 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-light-medium.css
--rw-r--r--   0 danvk      (501) staff       (20)     1450 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-light-soft.css
--rw-r--r--   0 danvk      (501) staff       (20)     1374 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/hardcore.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/harmonic16-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1413 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/harmonic16-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/heetch-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1399 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/heetch-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/helios.css
--rw-r--r--   0 danvk      (501) staff       (20)     1374 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/hopscotch.css
--rw-r--r--   0 danvk      (501) staff       (20)     1413 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/horizon-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/horizon-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1388 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/humanoid-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1389 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/humanoid-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1386 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ia-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1396 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ia-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1390 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/icy-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ir-black.css
--rw-r--r--   0 danvk      (501) staff       (20)     1334 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/isotope.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/kimber.css
--rw-r--r--   0 danvk      (501) staff       (20)     1376 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/london-tube.css
--rw-r--r--   0 danvk      (501) staff       (20)     1389 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/macintosh.css
--rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/marrakesh.css
--rw-r--r--   0 danvk      (501) staff       (20)     1363 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/materia.css
--rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/material-darker.css
--rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/material-lighter.css
--rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/material-palenight.css
--rw-r--r--   0 danvk      (501) staff       (20)     1378 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/material-vivid.css
--rw-r--r--   0 danvk      (501) staff       (20)     1366 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/material.css
--rw-r--r--   0 danvk      (501) staff       (20)     1363 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/mellow-purple.css
--rw-r--r--   0 danvk      (501) staff       (20)     1381 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/mexico-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/mocha.css
--rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/monokai.css
--rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/nebula.css
--rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/nord.css
--rw-r--r--   0 danvk      (501) staff       (20)     1430 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/nova.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ocean.css
--rw-r--r--   0 danvk      (501) staff       (20)     1418 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/oceanicnext.css
--rw-r--r--   0 danvk      (501) staff       (20)     1410 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/one-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1403 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/onedark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1416 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/outrun-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1476 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/papercolor-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1460 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/papercolor-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1372 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/paraiso.css
--rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/pasque.css
--rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/phd.css
--rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/pico.css
--rw-r--r--   0 danvk      (501) staff       (20)     1390 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/pop.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/porple.css
--rw-r--r--   0 danvk      (501) staff       (20)     1363 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/qualia.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/railscasts.css
--rw-r--r--   0 danvk      (501) staff       (20)     1455 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/rebecca.css
--rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ros-pine-dawn.css
--rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ros-pine-moon.css
--rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/ros-pine.css
--rw-r--r--   0 danvk      (501) staff       (20)     1380 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/sagelight.css
--rw-r--r--   0 danvk      (501) staff       (20)     1376 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/sandcastle.css
--rw-r--r--   0 danvk      (501) staff       (20)     1361 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/seti-ui.css
--rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/shapeshifter.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/silk-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1410 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/silk-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1476 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/snazzy.css
--rw-r--r--   0 danvk      (501) staff       (20)     1413 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/solar-flare-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1407 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/solar-flare.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/solarized-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/solarized-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1425 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/spacemacs.css
--rw-r--r--   0 danvk      (501) staff       (20)     1392 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/summercamp.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/summerfruit-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1404 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/summerfruit-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1429 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/synth-midnight-terminal-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1430 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/synth-midnight-terminal-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/tango.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/tender.css
--rw-r--r--   0 danvk      (501) staff       (20)     1374 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/tomorrow-night.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/tomorrow.css
--rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/twilight.css
--rw-r--r--   0 danvk      (501) staff       (20)     1393 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/unikitty-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1391 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/unikitty-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1350 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/vulcan.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-10-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1399 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-10.css
--rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-95-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1405 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-95.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-high-contrast-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-high-contrast.css
--rw-r--r--   0 danvk      (501) staff       (20)     1380 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-nt-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1367 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/windows-nt.css
--rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/woodland.css
--rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/xcode-dusk.css
--rw-r--r--   0 danvk      (501) staff       (20)     1361 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/base16/zenburn.css
--rw-r--r--   0 danvk      (501) staff       (20)      656 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/brown-paper.css
--rw-r--r--   0 danvk      (501) staff       (20)    18198 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/brown-papersq.png
--rw-r--r--   0 danvk      (501) staff       (20)      600 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/codepen-embed.css
--rw-r--r--   0 danvk      (501) staff       (20)      631 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/color-brewer.css
--rw-r--r--   0 danvk      (501) staff       (20)      625 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1144 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/default.css
--rw-r--r--   0 danvk      (501) staff       (20)     1080 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/devibeans.css
--rw-r--r--   0 danvk      (501) staff       (20)      837 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/docco.css
--rw-r--r--   0 danvk      (501) staff       (20)      669 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/far.css
--rw-r--r--   0 danvk      (501) staff       (20)     1169 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/felipec.css
--rw-r--r--   0 danvk      (501) staff       (20)      779 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/foundation.css
--rw-r--r--   0 danvk      (501) staff       (20)     1251 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/github-dark-dimmed.css
--rw-r--r--   0 danvk      (501) staff       (20)     1315 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/github-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1309 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/github.css
--rw-r--r--   0 danvk      (501) staff       (20)      787 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/gml.css
--rw-r--r--   0 danvk      (501) staff       (20)      835 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/googlecode.css
--rw-r--r--   0 danvk      (501) staff       (20)     1089 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/gradient-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1112 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/gradient-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     1674 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/grayscale.css
--rw-r--r--   0 danvk      (501) staff       (20)      897 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/hybrid.css
--rw-r--r--   0 danvk      (501) staff       (20)      906 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/idea.css
--rw-r--r--   0 danvk      (501) staff       (20)     1051 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/intellij-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      694 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/ir-black.css
--rw-r--r--   0 danvk      (501) staff       (20)      971 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/isbl-editor-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)      952 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/isbl-editor-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      652 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/kimbie-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)      652 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/kimbie-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      831 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/lightfair.css
--rw-r--r--   0 danvk      (501) staff       (20)      715 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/lioshi.css
--rw-r--r--   0 danvk      (501) staff       (20)      642 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/magula.css
--rw-r--r--   0 danvk      (501) staff       (20)      631 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/mono-blue.css
--rw-r--r--   0 danvk      (501) staff       (20)      826 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/monokai-sublime.css
--rw-r--r--   0 danvk      (501) staff       (20)      790 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/monokai.css
--rw-r--r--   0 danvk      (501) staff       (20)     1421 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/night-owl.css
--rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/nnfx-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/nnfx-light.css
--rw-r--r--   0 danvk      (501) staff       (20)     2684 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/nord.css
--rw-r--r--   0 danvk      (501) staff       (20)      882 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/obsidian.css
--rw-r--r--   0 danvk      (501) staff       (20)     1095 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/panda-syntax-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1069 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/panda-syntax-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      637 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/paraiso-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)      637 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/paraiso-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      814 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/pojoaque.css
--rw-r--r--   0 danvk      (501) staff       (20)     1186 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/pojoaque.jpg
--rw-r--r--   0 danvk      (501) staff       (20)      734 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/purebasic.css
--rw-r--r--   0 danvk      (501) staff       (20)      815 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/qtcreator-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)      810 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/qtcreator-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      826 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/rainbow.css
--rw-r--r--   0 danvk      (501) staff       (20)      862 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/routeros.css
--rw-r--r--   0 danvk      (501) staff       (20)      664 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/school-book.css
--rw-r--r--   0 danvk      (501) staff       (20)      854 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/shades-of-purple.css
--rw-r--r--   0 danvk      (501) staff       (20)      795 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/srcery.css
--rw-r--r--   0 danvk      (501) staff       (20)     1271 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/stackoverflow-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1285 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/stackoverflow-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      950 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/sunburst.css
--rw-r--r--   0 danvk      (501) staff       (20)     1234 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/tokyo-night-dark.css
--rw-r--r--   0 danvk      (501) staff       (20)     1235 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/tokyo-night-light.css
--rw-r--r--   0 danvk      (501) staff       (20)      648 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/tomorrow-night-blue.css
--rw-r--r--   0 danvk      (501) staff       (20)      648 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/tomorrow-night-bright.css
--rw-r--r--   0 danvk      (501) staff       (20)      640 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/vs.css
--rw-r--r--   0 danvk      (501) staff       (20)     1088 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/vs2015.css
--rw-r--r--   0 danvk      (501) staff       (20)      945 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/xcode.css
--rw-r--r--   0 danvk      (501) staff       (20)      765 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/css/themes/xt256.css
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.503449 webdiff-1.0.0/webdiff/static/img/
--rw-r--r--   0 danvk      (501) staff       (20)    67646 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/img/favicon.ico
--rw-r--r--   0 danvk      (501) staff       (20)     4450 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/img/sprites.png
--rw-r--r--   0 danvk      (501) staff       (20)       58 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/img/trans_bg.gif
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.510286 webdiff-1.0.0/webdiff/static/js/
--rw-r--r--   0 danvk      (501) staff       (20)   300303 2024-05-29 21:48:15.000000 webdiff-1.0.0/webdiff/static/js/file_diff.js
--rw-r--r--   0 danvk      (501) staff       (20)   984465 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/static/js/highlight.min.js
--rw-r--r--   0 danvk      (501) staff       (20)   749329 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/js/highlight.pack.min.js
--rw-r--r--   0 danvk      (501) staff       (20)    84245 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/static/js/jquery-2.1.1.min.js
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.517247 webdiff-1.0.0/webdiff/templates/
--rw-r--r--   0 danvk      (501) staff       (20)        0 2022-09-06 14:09:42.000000 webdiff-1.0.0/webdiff/templates/__init__.py
--rw-r--r--   0 danvk      (501) staff       (20)      683 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/templates/base.html
--rw-r--r--   0 danvk      (501) staff       (20)      479 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/templates/file_diff.html
--rw-r--r--   0 danvk      (501) staff       (20)     5164 2024-05-29 21:42:14.000000 webdiff-1.0.0/webdiff/unified_diff.py
--rw-r--r--   0 danvk      (501) staff       (20)     4129 2024-05-28 21:57:45.000000 webdiff-1.0.0/webdiff/util.py
-drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:08:17.519114 webdiff-1.0.0/webdiff.egg-info/
--rw-r--r--   0 danvk      (501) staff       (20)     8144 2024-05-30 20:08:17.000000 webdiff-1.0.0/webdiff.egg-info/PKG-INFO
--rw-r--r--   0 danvk      (501) staff       (20)    13078 2024-05-30 20:08:17.000000 webdiff-1.0.0/webdiff.egg-info/SOURCES.txt
--rw-r--r--   0 danvk      (501) staff       (20)        1 2024-05-30 20:08:17.000000 webdiff-1.0.0/webdiff.egg-info/dependency_links.txt
--rw-r--r--   0 danvk      (501) staff       (20)       81 2024-05-30 20:08:17.000000 webdiff-1.0.0/webdiff.egg-info/entry_points.txt
--rw-r--r--   0 danvk      (501) staff       (20)       87 2024-05-30 20:08:17.000000 webdiff-1.0.0/webdiff.egg-info/requires.txt
--rw-r--r--   0 danvk      (501) staff       (20)        8 2024-05-30 20:08:17.000000 webdiff-1.0.0/webdiff.egg-info/top_level.txt
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.980342 webdiff-1.0.1/
+-rw-r--r--   0 danvk      (501) staff       (20)    11323 2022-09-06 14:09:42.000000 webdiff-1.0.1/LICENSE
+-rw-r--r--   0 danvk      (501) staff       (20)       91 2022-09-06 14:09:42.000000 webdiff-1.0.1/MANIFEST.in
+-rw-r--r--   0 danvk      (501) staff       (20)     8318 2024-05-30 20:12:34.979819 webdiff-1.0.1/PKG-INFO
+-rw-r--r--   0 danvk      (501) staff       (20)     7551 2024-05-30 20:11:30.000000 webdiff-1.0.1/README.md
+-rw-r--r--   0 danvk      (501) staff       (20)       38 2024-05-30 20:12:34.980376 webdiff-1.0.1/setup.cfg
+-rw-r--r--   0 danvk      (501) staff       (20)     1381 2024-05-30 20:11:46.000000 webdiff-1.0.1/setup.py
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.931629 webdiff-1.0.1/webdiff/
+-rw-r--r--   0 danvk      (501) staff       (20)        0 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/__init__.py
+-rwxr-xr-x   0 danvk      (501) staff       (20)     9698 2024-05-30 20:12:17.000000 webdiff-1.0.1/webdiff/app.py
+-rw-r--r--   0 danvk      (501) staff       (20)     3708 2024-05-30 19:50:00.000000 webdiff-1.0.1/webdiff/argparser.py
+-rw-r--r--   0 danvk      (501) staff       (20)     4934 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/diff.py
+-rw-r--r--   0 danvk      (501) staff       (20)     2770 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/dirdiff.py
+-rw-r--r--   0 danvk      (501) staff       (20)     4439 2024-05-30 19:46:15.000000 webdiff-1.0.1/webdiff/github_fetcher.py
+-rw-r--r--   0 danvk      (501) staff       (20)     2254 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/githubdiff.py
+-rwxr-xr-x   0 danvk      (501) staff       (20)     1019 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/gitwebdiff.py
+-rw-r--r--   0 danvk      (501) staff       (20)     1809 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/localfilediff.py
+-rw-r--r--   0 danvk      (501) staff       (20)     1632 2024-05-30 15:27:35.000000 webdiff-1.0.1/webdiff/options.py
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.932435 webdiff-1.0.1/webdiff/static/
+-rw-r--r--   0 danvk      (501) staff       (20)        0 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/__init__.py
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.933037 webdiff-1.0.1/webdiff/static/codediff.js/
+-rw-r--r--   0 danvk      (501) staff       (20)     2807 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/codediff.js/codediff.css
+-rw-r--r--   0 danvk      (501) staff       (20)    22168 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/codediff.js/codediff.js
+-rwxr-xr-x   0 danvk      (501) staff       (20)    11308 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/codediff.js/difflib.js
+-rw-r--r--   0 danvk      (501) staff       (20)     2162 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/codediff.js/googlecode.css
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.933648 webdiff-1.0.1/webdiff/static/css/
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.934248 webdiff-1.0.1/webdiff/static/css/Inconsolata/
+-rwxr-xr-x   0 danvk      (501) staff       (20)    67724 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/css/Inconsolata/Inconsolata-Bold.ttf
+-rwxr-xr-x   0 danvk      (501) staff       (20)    84868 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/css/Inconsolata/Inconsolata-Regular.ttf
+-rwxr-xr-x   0 danvk      (501) staff       (20)     4498 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/css/Inconsolata/OFL.txt
+-rw-r--r--   0 danvk      (501) staff       (20)     1053 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/css/googlecode.css
+-rw-r--r--   0 danvk      (501) staff       (20)      189 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/css/inconsolata.css
+-rw-r--r--   0 danvk      (501) staff       (20)     3239 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/style.css
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.944879 webdiff-1.0.1/webdiff/static/css/themes/
+-rw-r--r--   0 danvk      (501) staff       (20)     1158 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/a11y-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1146 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/a11y-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1357 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/agate.css
+-rw-r--r--   0 danvk      (501) staff       (20)      961 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/an-old-hope.css
+-rw-r--r--   0 danvk      (501) staff       (20)      611 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/androidstudio.css
+-rw-r--r--   0 danvk      (501) staff       (20)      844 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/arduino-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      673 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/arta.css
+-rw-r--r--   0 danvk      (501) staff       (20)      454 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/ascetic.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1193 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/atom-one-dark-reasonable.css
+-rw-r--r--   0 danvk      (501) staff       (20)      856 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/atom-one-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)      856 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/atom-one-light.css
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.969917 webdiff-1.0.1/webdiff/static/css/themes/base16/
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/3024.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1403 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/apathy.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1368 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/apprentice.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ashes.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-cave-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-cave.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-dune-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-dune.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-estuary-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-estuary.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1416 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-forest-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1410 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-forest.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-heath-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-heath.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1418 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-lakeside-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-lakeside.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-plateau-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-plateau.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-savanna-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-savanna.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1417 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-seaside-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-seaside.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1421 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-sulphurpool-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1415 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-sulphurpool.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1391 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/atlas.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1368 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/bespin.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-bathory.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1375 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-burzum.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1390 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-dark-funeral.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1387 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-gorgoroth.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1377 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-immortal.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-khold.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1384 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-marduk.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1384 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-mayhem.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-nile.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-venom.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1372 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1404 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/brewer.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1396 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/bright.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1407 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/brogrammer.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/brush-trees-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1407 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/brush-trees.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/chalk.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1451 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/circus.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1400 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/classic-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/classic-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/codeschool.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1361 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/colors.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1400 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/cupcake.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1347 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/cupertino.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/danqing.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1367 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/darcula.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/dark-violet.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/darkmoss.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/darktooth.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/decaf.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1405 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/default-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/default-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/dirtysea.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1456 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/dracula.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1387 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/edge-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1388 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/edge-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1380 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/eighties.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1403 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/embers.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1382 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1381 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-gray-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-gray-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1424 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/espresso.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1396 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/eva-dim.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/eva.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/flat.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1394 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/framer.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1369 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/fruit-soda.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1404 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gigavolt.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1339 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/github.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1387 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/google-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/google-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/grayscale-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/grayscale-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1354 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/green-screen.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1449 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-hard.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1451 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-medium.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1449 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-pale.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1449 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-soft.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1450 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-light-hard.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1452 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-light-medium.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1450 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-light-soft.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1374 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/hardcore.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/harmonic16-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1413 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/harmonic16-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/heetch-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1399 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/heetch-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/helios.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1374 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/hopscotch.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1413 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/horizon-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/horizon-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1388 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/humanoid-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1389 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/humanoid-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1386 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ia-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1396 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ia-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1390 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/icy-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ir-black.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1334 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/isotope.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/kimber.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1376 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/london-tube.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1389 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/macintosh.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1408 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/marrakesh.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1363 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/materia.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/material-darker.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1383 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/material-lighter.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1385 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/material-palenight.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1378 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/material-vivid.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1366 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/material.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1363 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/mellow-purple.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1381 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/mexico-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/mocha.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/monokai.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/nebula.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1373 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/nord.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1430 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/nova.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ocean.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1418 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/oceanicnext.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1410 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/one-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1403 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/onedark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1416 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/outrun-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1476 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/papercolor-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1460 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/papercolor-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1372 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/paraiso.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1406 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/pasque.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/phd.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/pico.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1390 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/pop.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/porple.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1363 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/qualia.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/railscasts.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1455 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/rebecca.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ros-pine-dawn.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1402 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ros-pine-moon.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/ros-pine.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1380 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/sagelight.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1376 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/sandcastle.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1361 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/seti-ui.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1397 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/shapeshifter.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/silk-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1410 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/silk-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1476 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/snazzy.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1413 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/solar-flare-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1407 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/solar-flare.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/solarized-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/solarized-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1425 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/spacemacs.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1392 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/summercamp.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/summerfruit-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1404 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/summerfruit-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1429 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/synth-midnight-terminal-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1430 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/synth-midnight-terminal-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/tango.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/tender.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1374 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/tomorrow-night.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/tomorrow.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1401 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/twilight.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1393 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/unikitty-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1391 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/unikitty-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1350 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/vulcan.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-10-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1399 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-10.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1414 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-95-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1405 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-95.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-high-contrast-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-high-contrast.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1380 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-nt-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1367 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/windows-nt.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1398 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/woodland.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1409 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/xcode-dusk.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1361 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/base16/zenburn.css
+-rw-r--r--   0 danvk      (501) staff       (20)      656 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/brown-paper.css
+-rw-r--r--   0 danvk      (501) staff       (20)    18198 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/brown-papersq.png
+-rw-r--r--   0 danvk      (501) staff       (20)      600 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/codepen-embed.css
+-rw-r--r--   0 danvk      (501) staff       (20)      631 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/color-brewer.css
+-rw-r--r--   0 danvk      (501) staff       (20)      625 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1144 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/default.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1080 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/devibeans.css
+-rw-r--r--   0 danvk      (501) staff       (20)      837 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/docco.css
+-rw-r--r--   0 danvk      (501) staff       (20)      669 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/far.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1169 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/felipec.css
+-rw-r--r--   0 danvk      (501) staff       (20)      779 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/foundation.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1251 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/github-dark-dimmed.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1315 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/github-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1309 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/github.css
+-rw-r--r--   0 danvk      (501) staff       (20)      787 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/gml.css
+-rw-r--r--   0 danvk      (501) staff       (20)      835 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/googlecode.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1089 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/gradient-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1112 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/gradient-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1674 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/grayscale.css
+-rw-r--r--   0 danvk      (501) staff       (20)      897 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/hybrid.css
+-rw-r--r--   0 danvk      (501) staff       (20)      906 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/idea.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1051 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/intellij-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      694 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/ir-black.css
+-rw-r--r--   0 danvk      (501) staff       (20)      971 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/isbl-editor-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)      952 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/isbl-editor-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      652 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/kimbie-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)      652 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/kimbie-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      831 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/lightfair.css
+-rw-r--r--   0 danvk      (501) staff       (20)      715 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/lioshi.css
+-rw-r--r--   0 danvk      (501) staff       (20)      642 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/magula.css
+-rw-r--r--   0 danvk      (501) staff       (20)      631 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/mono-blue.css
+-rw-r--r--   0 danvk      (501) staff       (20)      826 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/monokai-sublime.css
+-rw-r--r--   0 danvk      (501) staff       (20)      790 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/monokai.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1421 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/night-owl.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1411 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/nnfx-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1412 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/nnfx-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)     2684 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/nord.css
+-rw-r--r--   0 danvk      (501) staff       (20)      882 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/obsidian.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1095 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/panda-syntax-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1069 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/panda-syntax-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      637 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/paraiso-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)      637 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/paraiso-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      814 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/pojoaque.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1186 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/pojoaque.jpg
+-rw-r--r--   0 danvk      (501) staff       (20)      734 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/purebasic.css
+-rw-r--r--   0 danvk      (501) staff       (20)      815 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/qtcreator-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)      810 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/qtcreator-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      826 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/rainbow.css
+-rw-r--r--   0 danvk      (501) staff       (20)      862 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/routeros.css
+-rw-r--r--   0 danvk      (501) staff       (20)      664 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/school-book.css
+-rw-r--r--   0 danvk      (501) staff       (20)      854 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/shades-of-purple.css
+-rw-r--r--   0 danvk      (501) staff       (20)      795 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/srcery.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1271 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/stackoverflow-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1285 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/stackoverflow-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      950 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/sunburst.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1234 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/tokyo-night-dark.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1235 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/tokyo-night-light.css
+-rw-r--r--   0 danvk      (501) staff       (20)      648 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/tomorrow-night-blue.css
+-rw-r--r--   0 danvk      (501) staff       (20)      648 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/tomorrow-night-bright.css
+-rw-r--r--   0 danvk      (501) staff       (20)      640 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/vs.css
+-rw-r--r--   0 danvk      (501) staff       (20)     1088 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/vs2015.css
+-rw-r--r--   0 danvk      (501) staff       (20)      945 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/xcode.css
+-rw-r--r--   0 danvk      (501) staff       (20)      765 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/css/themes/xt256.css
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.970438 webdiff-1.0.1/webdiff/static/img/
+-rw-r--r--   0 danvk      (501) staff       (20)    67646 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/img/favicon.ico
+-rw-r--r--   0 danvk      (501) staff       (20)     4450 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/img/sprites.png
+-rw-r--r--   0 danvk      (501) staff       (20)       58 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/img/trans_bg.gif
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.977117 webdiff-1.0.1/webdiff/static/js/
+-rw-r--r--   0 danvk      (501) staff       (20)   300303 2024-05-29 21:48:15.000000 webdiff-1.0.1/webdiff/static/js/file_diff.js
+-rw-r--r--   0 danvk      (501) staff       (20)   984465 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/static/js/highlight.min.js
+-rw-r--r--   0 danvk      (501) staff       (20)   749329 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/js/highlight.pack.min.js
+-rw-r--r--   0 danvk      (501) staff       (20)    84245 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/static/js/jquery-2.1.1.min.js
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.979191 webdiff-1.0.1/webdiff/templates/
+-rw-r--r--   0 danvk      (501) staff       (20)        0 2022-09-06 14:09:42.000000 webdiff-1.0.1/webdiff/templates/__init__.py
+-rw-r--r--   0 danvk      (501) staff       (20)      683 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/templates/base.html
+-rw-r--r--   0 danvk      (501) staff       (20)      479 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/templates/file_diff.html
+-rw-r--r--   0 danvk      (501) staff       (20)     5164 2024-05-29 21:42:14.000000 webdiff-1.0.1/webdiff/unified_diff.py
+-rw-r--r--   0 danvk      (501) staff       (20)     4129 2024-05-28 21:57:45.000000 webdiff-1.0.1/webdiff/util.py
+drwxr-xr-x   0 danvk      (501) staff       (20)        0 2024-05-30 20:12:34.979429 webdiff-1.0.1/webdiff.egg-info/
+-rw-r--r--   0 danvk      (501) staff       (20)     8318 2024-05-30 20:12:34.000000 webdiff-1.0.1/webdiff.egg-info/PKG-INFO
+-rw-r--r--   0 danvk      (501) staff       (20)    13078 2024-05-30 20:12:34.000000 webdiff-1.0.1/webdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 danvk      (501) staff       (20)        1 2024-05-30 20:12:34.000000 webdiff-1.0.1/webdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 danvk      (501) staff       (20)       81 2024-05-30 20:12:34.000000 webdiff-1.0.1/webdiff.egg-info/entry_points.txt
+-rw-r--r--   0 danvk      (501) staff       (20)       87 2024-05-30 20:12:34.000000 webdiff-1.0.1/webdiff.egg-info/requires.txt
+-rw-r--r--   0 danvk      (501) staff       (20)        8 2024-05-30 20:12:34.000000 webdiff-1.0.1/webdiff.egg-info/top_level.txt
```

### Comparing `webdiff-1.0.0/LICENSE` & `webdiff-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/PKG-INFO` & `webdiff-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdiff
-Version: 1.0.0
+Version: 1.0.1
 Summary: Two-column web-based git difftool
 Home-page: https://github.com/danvk/webdiff/
 Author: Dan Vanderkam
 Author-email: danvdk@gmail.com
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
@@ -37,19 +37,20 @@
 
 * Side-by-side (two column) diff view
 * Runs in the browser of your choice on any platform.
 * Syntax highlighting via highlight.js
 * Step back and forth through multiple files in a single diff
 * Rich support for image diffs
 
+<!-- These are absolute URLs so that they display on pypi.org -->
 <!-- This is `git webdiff 05157bba^..05157bba`, in this repo -->
-![Screenshot of webdiff in action](/images/webdiff.png)
+![Screenshot of webdiff in action](https://raw.githubusercontent.com/danvk/webdiff/master/images/webdiff.png)
 
 <!-- This is `git webdiff c80f969^..c80f969` in the dygraphs-dpxdt repo -->
-![Screenshot of image diffs](/images/webdiff-images.png)
+![Screenshot of image diffs](https://raw.githubusercontent.com/danvk/webdiff/master/images/webdiff-images.png)
 
 ## Installation
 
     pip install webdiff
 
 or, if you prefer [Homebrew]:
```

#### html2text {}

```diff
@@ -1,57 +1,59 @@
-Metadata-Version: 2.1 Name: webdiff Version: 1.0.0 Summary: Two-column web-
+Metadata-Version: 2.1 Name: webdiff Version: 1.0.1 Summary: Two-column web-
 based git difftool Home-page: https://github.com/danvk/webdiff/ Author: Dan
 Vanderkam Author-email: danvdk@gmail.com Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Framework :: Flask
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Version Control Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: binaryornot
 Requires-Dist: flask==2.2.2 Requires-Dist: pillow Requires-Dist: requests
 Requires-Dist: PyGithub==1.55 Requires-Dist: unidiff==0.7.4 Requires-Dist:
 Werkzeug==2.2.2 # git webdiff Two-column web-based git difftool.
 _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_C_i_r_c_l_e_C_I_ _ð____]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_2_ _ð____]_[_S_p_o_n_s_o_r_:_ _O_n_ _G_i_t_H_u_b_ _ð___¸_]
 Features include: * Side-by-side (two column) diff view * Runs in the browser
 of your choice on any platform. * Syntax highlighting via highlight.js * Step
 back and forth through multiple files in a single diff * Rich support for image
-diffs ![Screenshot of webdiff in action](/images/webdiff.png) ![Screenshot of
-image diffs](/images/webdiff-images.png) ## Installation pip install webdiff
-or, if you prefer [Homebrew]: brew install danvk/webdiff/webdiff (the latter
-will also install [ImageMagick] as a recommended dependency.) ## Usage Instead
-of running "git diff", run: git webdiff You can also start webdiff via: git
-webdiff [args] You can pass all the same arguments that you would to `git
-diff`, e.g. `1234..5678` or `HEAD`. `webdiff` can also be invoked directly to
-diff two directories or files: webdiff webdiff You can also use `webdiff` to
-view GitHub pull requests: webdiff https://github.com/owner/repo/pull/123
-webdiff '#123' # if you're in a git repo with a github remote This will
-download the files relevant to the Pull Request and run `webdiff`. If you run
-into GitHub API quota limits or you'd like to use webdiff with private repos,
-you can set your credentials in a `.githubrc` file: user.login: yourusername
-user.token: your-personal-access-tokens Make sure you chmod this file to only
-be readable by yourself. You can generate a personal access token for webdiff
-via github.com â profile â Settings â Personal access tokens. Make sure
-to grant all the "repo" privileges. ## Configuration webdiff can be configured
-via [`git config`][git config]. To change the syntax highlighting theme, for
-example: git config webdiff.theme rainbow (You can find a list of supported
-themes in the [themes] directory.) As with any git configuration setting, these
-can be set globally or per-repo. Options are: | Setting | Default | Notes | | -
-------------- | ------------- | ------ | | webdiff.theme | googlecode | Syntax
-highlighting theme (see [themes] directory). | | webdiff.port | -1 | Port on
-which to serve webdiff. Default is random open port. This can be overridden
-with the `--port` command line flag or the `WEBDIFF_PORT` environment variable.
-| | webdiff.host | localhost | Host name on which to serve the webdiff UI. Use
-`0.0.0.0` to serve publicly. The special value `` uses your computer's network
-name. This can be overridden with the `--host` command line flag or the
-`WEBDIFF_HOST` environment variable. | | webdiff.maxDiffWidth | 100 | Maximum
-length of lines in the diff display. After this width, lines will wrap. | |
-webdiff.unified | 8 | Lines of context to display by default (`git diff -U`) |
-| webdiff.extraDirDiffArgs | "" | Any extra arguments to pass to `git diff`
-when diffing directories. | | webdiff.extraFileDiffArgs | "" | Any extra
-arguments to pass to `git diff` when diffing files. | | webdiff.openBrowser |
-true | Whether to automatically open the browser UI when you run webdiff. | |
+diffs ![Screenshot of webdiff in action](https://raw.githubusercontent.com/
+danvk/webdiff/master/images/webdiff.png) ![Screenshot of image diffs](https://
+raw.githubusercontent.com/danvk/webdiff/master/images/webdiff-images.png) ##
+Installation pip install webdiff or, if you prefer [Homebrew]: brew install
+danvk/webdiff/webdiff (the latter will also install [ImageMagick] as a
+recommended dependency.) ## Usage Instead of running "git diff", run: git
+webdiff You can also start webdiff via: git webdiff [args] You can pass all the
+same arguments that you would to `git diff`, e.g. `1234..5678` or `HEAD`.
+`webdiff` can also be invoked directly to diff two directories or files:
+webdiff webdiff You can also use `webdiff` to view GitHub pull requests:
+webdiff https://github.com/owner/repo/pull/123 webdiff '#123' # if you're in a
+git repo with a github remote This will download the files relevant to the Pull
+Request and run `webdiff`. If you run into GitHub API quota limits or you'd
+like to use webdiff with private repos, you can set your credentials in a
+`.githubrc` file: user.login: yourusername user.token: your-personal-access-
+tokens Make sure you chmod this file to only be readable by yourself. You can
+generate a personal access token for webdiff via github.com â profile â
+Settings â Personal access tokens. Make sure to grant all the "repo"
+privileges. ## Configuration webdiff can be configured via [`git config`][git
+config]. To change the syntax highlighting theme, for example: git config
+webdiff.theme rainbow (You can find a list of supported themes in the [themes]
+directory.) As with any git configuration setting, these can be set globally or
+per-repo. Options are: | Setting | Default | Notes | | -------------- | -------
+------ | ------ | | webdiff.theme | googlecode | Syntax highlighting theme (see
+[themes] directory). | | webdiff.port | -1 | Port on which to serve webdiff.
+Default is random open port. This can be overridden with the `--port` command
+line flag or the `WEBDIFF_PORT` environment variable. | | webdiff.host |
+localhost | Host name on which to serve the webdiff UI. Use `0.0.0.0` to serve
+publicly. The special value `` uses your computer's network name. This can be
+overridden with the `--host` command line flag or the `WEBDIFF_HOST`
+environment variable. | | webdiff.maxDiffWidth | 100 | Maximum length of lines
+in the diff display. After this width, lines will wrap. | | webdiff.unified | 8
+| Lines of context to display by default (`git diff -U`) | |
+webdiff.extraDirDiffArgs | "" | Any extra arguments to pass to `git diff` when
+diffing directories. | | webdiff.extraFileDiffArgs | "" | Any extra arguments
+to pass to `git diff` when diffing files. | | webdiff.openBrowser | true |
+Whether to automatically open the browser UI when you run webdiff. | |
 webdiff.maxLinesForSyntax | 10000 | Maximum lines in file to do syntax
 highlighting. | | webdiff.colors.delete | #fee | CSS background color for
 delete (left) lines | | webdiff.colors.insert | #efe | CSS background color for
 insert (right) lines | | webdiff.colors.charDelete | #fcc | CSS background
 color for deleted characters in a delete (left) line | |
 webdiff.colors.charInsert | #cfc | CSS background color for inserted characters
 in an insert (right) line | ## Development python3 -m venv venv source venv/
```

### Comparing `webdiff-1.0.0/README.md` & `webdiff-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 
 * Side-by-side (two column) diff view
 * Runs in the browser of your choice on any platform.
 * Syntax highlighting via highlight.js
 * Step back and forth through multiple files in a single diff
 * Rich support for image diffs
 
+<!-- These are absolute URLs so that they display on pypi.org -->
 <!-- This is `git webdiff 05157bba^..05157bba`, in this repo -->
-![Screenshot of webdiff in action](/images/webdiff.png)
+![Screenshot of webdiff in action](https://raw.githubusercontent.com/danvk/webdiff/master/images/webdiff.png)
 
 <!-- This is `git webdiff c80f969^..c80f969` in the dygraphs-dpxdt repo -->
-![Screenshot of image diffs](/images/webdiff-images.png)
+![Screenshot of image diffs](https://raw.githubusercontent.com/danvk/webdiff/master/images/webdiff-images.png)
 
 ## Installation
 
     pip install webdiff
 
 or, if you prefer [Homebrew]:
```

#### html2text {}

```diff
@@ -1,47 +1,49 @@
 # git webdiff Two-column web-based git difftool.
 _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_C_i_r_c_l_e_C_I_ _ð____]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_2_ _ð____]_[_S_p_o_n_s_o_r_:_ _O_n_ _G_i_t_H_u_b_ _ð___¸_]
 Features include: * Side-by-side (two column) diff view * Runs in the browser
 of your choice on any platform. * Syntax highlighting via highlight.js * Step
 back and forth through multiple files in a single diff * Rich support for image
-diffs ![Screenshot of webdiff in action](/images/webdiff.png) ![Screenshot of
-image diffs](/images/webdiff-images.png) ## Installation pip install webdiff
-or, if you prefer [Homebrew]: brew install danvk/webdiff/webdiff (the latter
-will also install [ImageMagick] as a recommended dependency.) ## Usage Instead
-of running "git diff", run: git webdiff You can also start webdiff via: git
-webdiff [args] You can pass all the same arguments that you would to `git
-diff`, e.g. `1234..5678` or `HEAD`. `webdiff` can also be invoked directly to
-diff two directories or files: webdiff webdiff You can also use `webdiff` to
-view GitHub pull requests: webdiff https://github.com/owner/repo/pull/123
-webdiff '#123' # if you're in a git repo with a github remote This will
-download the files relevant to the Pull Request and run `webdiff`. If you run
-into GitHub API quota limits or you'd like to use webdiff with private repos,
-you can set your credentials in a `.githubrc` file: user.login: yourusername
-user.token: your-personal-access-tokens Make sure you chmod this file to only
-be readable by yourself. You can generate a personal access token for webdiff
-via github.com â profile â Settings â Personal access tokens. Make sure
-to grant all the "repo" privileges. ## Configuration webdiff can be configured
-via [`git config`][git config]. To change the syntax highlighting theme, for
-example: git config webdiff.theme rainbow (You can find a list of supported
-themes in the [themes] directory.) As with any git configuration setting, these
-can be set globally or per-repo. Options are: | Setting | Default | Notes | | -
-------------- | ------------- | ------ | | webdiff.theme | googlecode | Syntax
-highlighting theme (see [themes] directory). | | webdiff.port | -1 | Port on
-which to serve webdiff. Default is random open port. This can be overridden
-with the `--port` command line flag or the `WEBDIFF_PORT` environment variable.
-| | webdiff.host | localhost | Host name on which to serve the webdiff UI. Use
-`0.0.0.0` to serve publicly. The special value `` uses your computer's network
-name. This can be overridden with the `--host` command line flag or the
-`WEBDIFF_HOST` environment variable. | | webdiff.maxDiffWidth | 100 | Maximum
-length of lines in the diff display. After this width, lines will wrap. | |
-webdiff.unified | 8 | Lines of context to display by default (`git diff -U`) |
-| webdiff.extraDirDiffArgs | "" | Any extra arguments to pass to `git diff`
-when diffing directories. | | webdiff.extraFileDiffArgs | "" | Any extra
-arguments to pass to `git diff` when diffing files. | | webdiff.openBrowser |
-true | Whether to automatically open the browser UI when you run webdiff. | |
+diffs ![Screenshot of webdiff in action](https://raw.githubusercontent.com/
+danvk/webdiff/master/images/webdiff.png) ![Screenshot of image diffs](https://
+raw.githubusercontent.com/danvk/webdiff/master/images/webdiff-images.png) ##
+Installation pip install webdiff or, if you prefer [Homebrew]: brew install
+danvk/webdiff/webdiff (the latter will also install [ImageMagick] as a
+recommended dependency.) ## Usage Instead of running "git diff", run: git
+webdiff You can also start webdiff via: git webdiff [args] You can pass all the
+same arguments that you would to `git diff`, e.g. `1234..5678` or `HEAD`.
+`webdiff` can also be invoked directly to diff two directories or files:
+webdiff webdiff You can also use `webdiff` to view GitHub pull requests:
+webdiff https://github.com/owner/repo/pull/123 webdiff '#123' # if you're in a
+git repo with a github remote This will download the files relevant to the Pull
+Request and run `webdiff`. If you run into GitHub API quota limits or you'd
+like to use webdiff with private repos, you can set your credentials in a
+`.githubrc` file: user.login: yourusername user.token: your-personal-access-
+tokens Make sure you chmod this file to only be readable by yourself. You can
+generate a personal access token for webdiff via github.com â profile â
+Settings â Personal access tokens. Make sure to grant all the "repo"
+privileges. ## Configuration webdiff can be configured via [`git config`][git
+config]. To change the syntax highlighting theme, for example: git config
+webdiff.theme rainbow (You can find a list of supported themes in the [themes]
+directory.) As with any git configuration setting, these can be set globally or
+per-repo. Options are: | Setting | Default | Notes | | -------------- | -------
+------ | ------ | | webdiff.theme | googlecode | Syntax highlighting theme (see
+[themes] directory). | | webdiff.port | -1 | Port on which to serve webdiff.
+Default is random open port. This can be overridden with the `--port` command
+line flag or the `WEBDIFF_PORT` environment variable. | | webdiff.host |
+localhost | Host name on which to serve the webdiff UI. Use `0.0.0.0` to serve
+publicly. The special value `` uses your computer's network name. This can be
+overridden with the `--host` command line flag or the `WEBDIFF_HOST`
+environment variable. | | webdiff.maxDiffWidth | 100 | Maximum length of lines
+in the diff display. After this width, lines will wrap. | | webdiff.unified | 8
+| Lines of context to display by default (`git diff -U`) | |
+webdiff.extraDirDiffArgs | "" | Any extra arguments to pass to `git diff` when
+diffing directories. | | webdiff.extraFileDiffArgs | "" | Any extra arguments
+to pass to `git diff` when diffing files. | | webdiff.openBrowser | true |
+Whether to automatically open the browser UI when you run webdiff. | |
 webdiff.maxLinesForSyntax | 10000 | Maximum lines in file to do syntax
 highlighting. | | webdiff.colors.delete | #fee | CSS background color for
 delete (left) lines | | webdiff.colors.insert | #efe | CSS background color for
 insert (right) lines | | webdiff.colors.charDelete | #fcc | CSS background
 color for deleted characters in a delete (left) line | |
 webdiff.colors.charInsert | #cfc | CSS background color for inserted characters
 in an insert (right) line | ## Development python3 -m venv venv source venv/
```

### Comparing `webdiff-1.0.0/setup.py` & `webdiff-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf8') as fh:
     long_description = fh.read()
 
 
 setup(name='webdiff',
-      version='1.0.0',
+      version='1.0.1',
       description='Two-column web-based git difftool',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Dan Vanderkam',
       author_email='danvdk@gmail.com',
       url='https://github.com/danvk/webdiff/',
       entry_points={
```

### Comparing `webdiff-1.0.0/webdiff/app.py` & `webdiff-1.0.1/webdiff/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 
 from webdiff import diff
 from webdiff import util
 from webdiff import argparser
 from webdiff import options
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 
 
 def determine_path():
     """Borrowed from wxglade.py"""
     try:
         root = __file__
         if os.path.islink(root):
```

### Comparing `webdiff-1.0.0/webdiff/argparser.py` & `webdiff-1.0.1/webdiff/argparser.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/diff.py` & `webdiff-1.0.1/webdiff/diff.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/dirdiff.py` & `webdiff-1.0.1/webdiff/dirdiff.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/github_fetcher.py` & `webdiff-1.0.1/webdiff/github_fetcher.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/githubdiff.py` & `webdiff-1.0.1/webdiff/githubdiff.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/gitwebdiff.py` & `webdiff-1.0.1/webdiff/gitwebdiff.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/localfilediff.py` & `webdiff-1.0.1/webdiff/localfilediff.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/options.py` & `webdiff-1.0.1/webdiff/options.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/codediff.js/codediff.css` & `webdiff-1.0.1/webdiff/static/codediff.js/codediff.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/codediff.js/codediff.js` & `webdiff-1.0.1/webdiff/static/codediff.js/codediff.js`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/codediff.js/difflib.js` & `webdiff-1.0.1/webdiff/static/codediff.js/difflib.js`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/codediff.js/googlecode.css` & `webdiff-1.0.1/webdiff/static/codediff.js/googlecode.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/Inconsolata/Inconsolata-Bold.ttf` & `webdiff-1.0.1/webdiff/static/css/Inconsolata/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/Inconsolata/Inconsolata-Regular.ttf` & `webdiff-1.0.1/webdiff/static/css/Inconsolata/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/Inconsolata/OFL.txt` & `webdiff-1.0.1/webdiff/static/css/Inconsolata/OFL.txt`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/googlecode.css` & `webdiff-1.0.1/webdiff/static/css/googlecode.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/style.css` & `webdiff-1.0.1/webdiff/static/css/style.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/a11y-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/a11y-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/a11y-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/a11y-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/agate.css` & `webdiff-1.0.1/webdiff/static/css/themes/agate.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/an-old-hope.css` & `webdiff-1.0.1/webdiff/static/css/themes/an-old-hope.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/androidstudio.css` & `webdiff-1.0.1/webdiff/static/css/themes/androidstudio.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/arduino-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/arduino-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/arta.css` & `webdiff-1.0.1/webdiff/static/css/themes/arta.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/atom-one-dark-reasonable.css` & `webdiff-1.0.1/webdiff/static/css/themes/atom-one-dark-reasonable.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/atom-one-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/atom-one-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/atom-one-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/atom-one-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/3024.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/3024.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/apathy.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/apathy.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/apprentice.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/apprentice.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ashes.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ashes.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-cave-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-cave-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-cave.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-cave.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-dune-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-dune-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-dune.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-dune.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-estuary-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-estuary-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-estuary.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-estuary.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-forest-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-forest-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-forest.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-forest.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-heath-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-heath-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-heath.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-heath.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-lakeside-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-lakeside-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-lakeside.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-lakeside.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-plateau-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-plateau-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-plateau.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-plateau.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-savanna-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-savanna-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-savanna.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-savanna.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-seaside-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-seaside-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-seaside.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-seaside.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-sulphurpool-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-sulphurpool-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atelier-sulphurpool.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atelier-sulphurpool.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/atlas.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/atlas.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/bespin.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/bespin.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-bathory.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-bathory.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-burzum.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-burzum.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-dark-funeral.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-dark-funeral.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-gorgoroth.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-gorgoroth.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-immortal.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-immortal.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-khold.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-khold.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-marduk.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-marduk.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-mayhem.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-mayhem.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-nile.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-nile.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal-venom.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal-venom.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/black-metal.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/black-metal.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/brewer.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/brewer.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/bright.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/bright.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/brogrammer.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/brogrammer.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/brush-trees-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/brush-trees-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/brush-trees.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/brush-trees.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/chalk.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/chalk.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/circus.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/circus.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/classic-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/classic-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/classic-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/classic-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/codeschool.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/codeschool.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/colors.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/colors.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/cupcake.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/cupcake.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/cupertino.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/cupertino.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/danqing.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/danqing.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/darcula.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/darcula.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/dark-violet.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/dark-violet.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/darkmoss.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/darkmoss.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/darktooth.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/darktooth.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/decaf.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/decaf.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/default-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/default-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/default-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/default-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/dirtysea.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/dirtysea.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/dracula.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/dracula.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/edge-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/edge-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/edge-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/edge-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/eighties.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/eighties.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/embers.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/embers.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-gray-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-gray-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-gray-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-gray-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/equilibrium-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/equilibrium-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/espresso.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/espresso.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/eva-dim.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/eva-dim.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/eva.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/eva.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/flat.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/flat.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/framer.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/framer.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/fruit-soda.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/fruit-soda.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gigavolt.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gigavolt.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/github.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/github.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/google-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/google-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/google-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/google-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/grayscale-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/grayscale-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/grayscale-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/grayscale-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/green-screen.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/green-screen.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-hard.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-hard.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-medium.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-medium.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-pale.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-pale.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-dark-soft.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-dark-soft.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-light-hard.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-light-hard.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-light-medium.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-light-medium.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/gruvbox-light-soft.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/gruvbox-light-soft.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/hardcore.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/hardcore.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/harmonic16-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/harmonic16-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/harmonic16-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/harmonic16-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/heetch-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/heetch-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/heetch-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/heetch-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/helios.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/helios.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/hopscotch.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/hopscotch.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/horizon-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/horizon-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/horizon-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/horizon-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/humanoid-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/humanoid-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/humanoid-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/humanoid-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ia-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ia-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ia-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ia-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/icy-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/icy-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ir-black.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ir-black.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/isotope.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/isotope.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/kimber.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/kimber.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/london-tube.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/london-tube.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/macintosh.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/macintosh.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/marrakesh.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/marrakesh.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/materia.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/materia.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/material-darker.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/material-darker.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/material-lighter.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/material-lighter.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/material-palenight.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/material-palenight.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/material-vivid.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/material-vivid.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/material.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/material.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/mellow-purple.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/mellow-purple.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/mexico-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/mexico-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/mocha.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/mocha.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/monokai.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/monokai.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/nebula.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/nebula.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/nord.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/nord.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/nova.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/nova.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ocean.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ocean.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/oceanicnext.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/oceanicnext.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/one-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/one-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/onedark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/onedark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/outrun-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/outrun-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/papercolor-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/papercolor-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/papercolor-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/papercolor-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/paraiso.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/paraiso.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/pasque.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/pasque.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/phd.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/phd.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/pico.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/pico.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/pop.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/pop.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/porple.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/porple.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/qualia.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/qualia.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/railscasts.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/railscasts.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/rebecca.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/rebecca.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ros-pine-dawn.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ros-pine-dawn.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ros-pine-moon.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ros-pine-moon.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/ros-pine.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/ros-pine.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/sagelight.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/sagelight.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/sandcastle.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/sandcastle.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/seti-ui.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/seti-ui.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/shapeshifter.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/shapeshifter.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/silk-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/silk-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/silk-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/silk-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/snazzy.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/snazzy.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/solar-flare-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/solar-flare-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/solar-flare.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/solar-flare.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/solarized-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/solarized-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/solarized-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/spacemacs.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/spacemacs.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/summercamp.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/summercamp.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/summerfruit-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/summerfruit-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/summerfruit-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/summerfruit-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/synth-midnight-terminal-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/synth-midnight-terminal-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/synth-midnight-terminal-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/synth-midnight-terminal-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/tango.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/tango.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/tender.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/tender.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/tomorrow-night.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/tomorrow-night.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/tomorrow.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/tomorrow.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/twilight.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/twilight.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/unikitty-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/unikitty-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/unikitty-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/unikitty-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/vulcan.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/vulcan.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-10-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-10-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-10.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-10.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-95-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-95-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-95.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-95.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-high-contrast-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-high-contrast-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-high-contrast.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-high-contrast.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-nt-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-nt-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/windows-nt.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/windows-nt.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/woodland.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/woodland.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/xcode-dusk.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/xcode-dusk.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/base16/zenburn.css` & `webdiff-1.0.1/webdiff/static/css/themes/base16/zenburn.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/brown-paper.css` & `webdiff-1.0.1/webdiff/static/css/themes/brown-paper.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/brown-papersq.png` & `webdiff-1.0.1/webdiff/static/css/themes/brown-papersq.png`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/codepen-embed.css` & `webdiff-1.0.1/webdiff/static/css/themes/codepen-embed.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/color-brewer.css` & `webdiff-1.0.1/webdiff/static/css/themes/color-brewer.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/default.css` & `webdiff-1.0.1/webdiff/static/css/themes/default.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/devibeans.css` & `webdiff-1.0.1/webdiff/static/css/themes/devibeans.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/docco.css` & `webdiff-1.0.1/webdiff/static/css/themes/docco.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/far.css` & `webdiff-1.0.1/webdiff/static/css/themes/far.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/felipec.css` & `webdiff-1.0.1/webdiff/static/css/themes/felipec.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/foundation.css` & `webdiff-1.0.1/webdiff/static/css/themes/foundation.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/github-dark-dimmed.css` & `webdiff-1.0.1/webdiff/static/css/themes/github-dark-dimmed.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/github-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/github-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/github.css` & `webdiff-1.0.1/webdiff/static/css/themes/github.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/gml.css` & `webdiff-1.0.1/webdiff/static/css/themes/gml.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/googlecode.css` & `webdiff-1.0.1/webdiff/static/css/themes/googlecode.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/gradient-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/gradient-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/gradient-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/gradient-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/grayscale.css` & `webdiff-1.0.1/webdiff/static/css/themes/grayscale.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/hybrid.css` & `webdiff-1.0.1/webdiff/static/css/themes/hybrid.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/idea.css` & `webdiff-1.0.1/webdiff/static/css/themes/idea.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/intellij-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/intellij-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/ir-black.css` & `webdiff-1.0.1/webdiff/static/css/themes/ir-black.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/isbl-editor-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/isbl-editor-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/isbl-editor-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/isbl-editor-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/kimbie-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/kimbie-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/kimbie-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/kimbie-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/lightfair.css` & `webdiff-1.0.1/webdiff/static/css/themes/lightfair.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/lioshi.css` & `webdiff-1.0.1/webdiff/static/css/themes/lioshi.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/magula.css` & `webdiff-1.0.1/webdiff/static/css/themes/magula.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/mono-blue.css` & `webdiff-1.0.1/webdiff/static/css/themes/mono-blue.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/monokai-sublime.css` & `webdiff-1.0.1/webdiff/static/css/themes/monokai-sublime.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/monokai.css` & `webdiff-1.0.1/webdiff/static/css/themes/monokai.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/night-owl.css` & `webdiff-1.0.1/webdiff/static/css/themes/night-owl.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/nnfx-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/nnfx-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/nnfx-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/nnfx-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/nord.css` & `webdiff-1.0.1/webdiff/static/css/themes/nord.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/obsidian.css` & `webdiff-1.0.1/webdiff/static/css/themes/obsidian.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/panda-syntax-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/panda-syntax-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/panda-syntax-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/panda-syntax-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/paraiso-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/paraiso-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/pojoaque.css` & `webdiff-1.0.1/webdiff/static/css/themes/pojoaque.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/pojoaque.jpg` & `webdiff-1.0.1/webdiff/static/css/themes/pojoaque.jpg`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/purebasic.css` & `webdiff-1.0.1/webdiff/static/css/themes/purebasic.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/qtcreator-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/qtcreator-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/qtcreator-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/qtcreator-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/rainbow.css` & `webdiff-1.0.1/webdiff/static/css/themes/rainbow.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/routeros.css` & `webdiff-1.0.1/webdiff/static/css/themes/routeros.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/school-book.css` & `webdiff-1.0.1/webdiff/static/css/themes/school-book.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/shades-of-purple.css` & `webdiff-1.0.1/webdiff/static/css/themes/shades-of-purple.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/srcery.css` & `webdiff-1.0.1/webdiff/static/css/themes/srcery.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/stackoverflow-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/stackoverflow-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/stackoverflow-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/stackoverflow-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/sunburst.css` & `webdiff-1.0.1/webdiff/static/css/themes/sunburst.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/tokyo-night-dark.css` & `webdiff-1.0.1/webdiff/static/css/themes/tokyo-night-dark.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/tokyo-night-light.css` & `webdiff-1.0.1/webdiff/static/css/themes/tokyo-night-light.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/tomorrow-night-blue.css` & `webdiff-1.0.1/webdiff/static/css/themes/tomorrow-night-blue.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/tomorrow-night-bright.css` & `webdiff-1.0.1/webdiff/static/css/themes/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/vs.css` & `webdiff-1.0.1/webdiff/static/css/themes/vs.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/vs2015.css` & `webdiff-1.0.1/webdiff/static/css/themes/vs2015.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/xcode.css` & `webdiff-1.0.1/webdiff/static/css/themes/xcode.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/css/themes/xt256.css` & `webdiff-1.0.1/webdiff/static/css/themes/xt256.css`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/img/favicon.ico` & `webdiff-1.0.1/webdiff/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/img/sprites.png` & `webdiff-1.0.1/webdiff/static/img/sprites.png`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/js/file_diff.js` & `webdiff-1.0.1/webdiff/static/js/file_diff.js`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/js/highlight.min.js` & `webdiff-1.0.1/webdiff/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/js/highlight.pack.min.js` & `webdiff-1.0.1/webdiff/static/js/highlight.pack.min.js`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/static/js/jquery-2.1.1.min.js` & `webdiff-1.0.1/webdiff/static/js/jquery-2.1.1.min.js`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/templates/base.html` & `webdiff-1.0.1/webdiff/templates/base.html`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/unified_diff.py` & `webdiff-1.0.1/webdiff/unified_diff.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff/util.py` & `webdiff-1.0.1/webdiff/util.py`

 * *Files identical despite different names*

### Comparing `webdiff-1.0.0/webdiff.egg-info/PKG-INFO` & `webdiff-1.0.1/webdiff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdiff
-Version: 1.0.0
+Version: 1.0.1
 Summary: Two-column web-based git difftool
 Home-page: https://github.com/danvk/webdiff/
 Author: Dan Vanderkam
 Author-email: danvdk@gmail.com
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
@@ -37,19 +37,20 @@
 
 * Side-by-side (two column) diff view
 * Runs in the browser of your choice on any platform.
 * Syntax highlighting via highlight.js
 * Step back and forth through multiple files in a single diff
 * Rich support for image diffs
 
+<!-- These are absolute URLs so that they display on pypi.org -->
 <!-- This is `git webdiff 05157bba^..05157bba`, in this repo -->
-![Screenshot of webdiff in action](/images/webdiff.png)
+![Screenshot of webdiff in action](https://raw.githubusercontent.com/danvk/webdiff/master/images/webdiff.png)
 
 <!-- This is `git webdiff c80f969^..c80f969` in the dygraphs-dpxdt repo -->
-![Screenshot of image diffs](/images/webdiff-images.png)
+![Screenshot of image diffs](https://raw.githubusercontent.com/danvk/webdiff/master/images/webdiff-images.png)
 
 ## Installation
 
     pip install webdiff
 
 or, if you prefer [Homebrew]:
```

#### html2text {}

```diff
@@ -1,57 +1,59 @@
-Metadata-Version: 2.1 Name: webdiff Version: 1.0.0 Summary: Two-column web-
+Metadata-Version: 2.1 Name: webdiff Version: 1.0.1 Summary: Two-column web-
 based git difftool Home-page: https://github.com/danvk/webdiff/ Author: Dan
 Vanderkam Author-email: danvdk@gmail.com Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Framework :: Flask
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Version Control Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: binaryornot
 Requires-Dist: flask==2.2.2 Requires-Dist: pillow Requires-Dist: requests
 Requires-Dist: PyGithub==1.55 Requires-Dist: unidiff==0.7.4 Requires-Dist:
 Werkzeug==2.2.2 # git webdiff Two-column web-based git difftool.
 _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_C_i_r_c_l_e_C_I_ _ð____]_[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_2_ _ð____]_[_S_p_o_n_s_o_r_:_ _O_n_ _G_i_t_H_u_b_ _ð___¸_]
 Features include: * Side-by-side (two column) diff view * Runs in the browser
 of your choice on any platform. * Syntax highlighting via highlight.js * Step
 back and forth through multiple files in a single diff * Rich support for image
-diffs ![Screenshot of webdiff in action](/images/webdiff.png) ![Screenshot of
-image diffs](/images/webdiff-images.png) ## Installation pip install webdiff
-or, if you prefer [Homebrew]: brew install danvk/webdiff/webdiff (the latter
-will also install [ImageMagick] as a recommended dependency.) ## Usage Instead
-of running "git diff", run: git webdiff You can also start webdiff via: git
-webdiff [args] You can pass all the same arguments that you would to `git
-diff`, e.g. `1234..5678` or `HEAD`. `webdiff` can also be invoked directly to
-diff two directories or files: webdiff webdiff You can also use `webdiff` to
-view GitHub pull requests: webdiff https://github.com/owner/repo/pull/123
-webdiff '#123' # if you're in a git repo with a github remote This will
-download the files relevant to the Pull Request and run `webdiff`. If you run
-into GitHub API quota limits or you'd like to use webdiff with private repos,
-you can set your credentials in a `.githubrc` file: user.login: yourusername
-user.token: your-personal-access-tokens Make sure you chmod this file to only
-be readable by yourself. You can generate a personal access token for webdiff
-via github.com â profile â Settings â Personal access tokens. Make sure
-to grant all the "repo" privileges. ## Configuration webdiff can be configured
-via [`git config`][git config]. To change the syntax highlighting theme, for
-example: git config webdiff.theme rainbow (You can find a list of supported
-themes in the [themes] directory.) As with any git configuration setting, these
-can be set globally or per-repo. Options are: | Setting | Default | Notes | | -
-------------- | ------------- | ------ | | webdiff.theme | googlecode | Syntax
-highlighting theme (see [themes] directory). | | webdiff.port | -1 | Port on
-which to serve webdiff. Default is random open port. This can be overridden
-with the `--port` command line flag or the `WEBDIFF_PORT` environment variable.
-| | webdiff.host | localhost | Host name on which to serve the webdiff UI. Use
-`0.0.0.0` to serve publicly. The special value `` uses your computer's network
-name. This can be overridden with the `--host` command line flag or the
-`WEBDIFF_HOST` environment variable. | | webdiff.maxDiffWidth | 100 | Maximum
-length of lines in the diff display. After this width, lines will wrap. | |
-webdiff.unified | 8 | Lines of context to display by default (`git diff -U`) |
-| webdiff.extraDirDiffArgs | "" | Any extra arguments to pass to `git diff`
-when diffing directories. | | webdiff.extraFileDiffArgs | "" | Any extra
-arguments to pass to `git diff` when diffing files. | | webdiff.openBrowser |
-true | Whether to automatically open the browser UI when you run webdiff. | |
+diffs ![Screenshot of webdiff in action](https://raw.githubusercontent.com/
+danvk/webdiff/master/images/webdiff.png) ![Screenshot of image diffs](https://
+raw.githubusercontent.com/danvk/webdiff/master/images/webdiff-images.png) ##
+Installation pip install webdiff or, if you prefer [Homebrew]: brew install
+danvk/webdiff/webdiff (the latter will also install [ImageMagick] as a
+recommended dependency.) ## Usage Instead of running "git diff", run: git
+webdiff You can also start webdiff via: git webdiff [args] You can pass all the
+same arguments that you would to `git diff`, e.g. `1234..5678` or `HEAD`.
+`webdiff` can also be invoked directly to diff two directories or files:
+webdiff webdiff You can also use `webdiff` to view GitHub pull requests:
+webdiff https://github.com/owner/repo/pull/123 webdiff '#123' # if you're in a
+git repo with a github remote This will download the files relevant to the Pull
+Request and run `webdiff`. If you run into GitHub API quota limits or you'd
+like to use webdiff with private repos, you can set your credentials in a
+`.githubrc` file: user.login: yourusername user.token: your-personal-access-
+tokens Make sure you chmod this file to only be readable by yourself. You can
+generate a personal access token for webdiff via github.com â profile â
+Settings â Personal access tokens. Make sure to grant all the "repo"
+privileges. ## Configuration webdiff can be configured via [`git config`][git
+config]. To change the syntax highlighting theme, for example: git config
+webdiff.theme rainbow (You can find a list of supported themes in the [themes]
+directory.) As with any git configuration setting, these can be set globally or
+per-repo. Options are: | Setting | Default | Notes | | -------------- | -------
+------ | ------ | | webdiff.theme | googlecode | Syntax highlighting theme (see
+[themes] directory). | | webdiff.port | -1 | Port on which to serve webdiff.
+Default is random open port. This can be overridden with the `--port` command
+line flag or the `WEBDIFF_PORT` environment variable. | | webdiff.host |
+localhost | Host name on which to serve the webdiff UI. Use `0.0.0.0` to serve
+publicly. The special value `` uses your computer's network name. This can be
+overridden with the `--host` command line flag or the `WEBDIFF_HOST`
+environment variable. | | webdiff.maxDiffWidth | 100 | Maximum length of lines
+in the diff display. After this width, lines will wrap. | | webdiff.unified | 8
+| Lines of context to display by default (`git diff -U`) | |
+webdiff.extraDirDiffArgs | "" | Any extra arguments to pass to `git diff` when
+diffing directories. | | webdiff.extraFileDiffArgs | "" | Any extra arguments
+to pass to `git diff` when diffing files. | | webdiff.openBrowser | true |
+Whether to automatically open the browser UI when you run webdiff. | |
 webdiff.maxLinesForSyntax | 10000 | Maximum lines in file to do syntax
 highlighting. | | webdiff.colors.delete | #fee | CSS background color for
 delete (left) lines | | webdiff.colors.insert | #efe | CSS background color for
 insert (right) lines | | webdiff.colors.charDelete | #fcc | CSS background
 color for deleted characters in a delete (left) line | |
 webdiff.colors.charInsert | #cfc | CSS background color for inserted characters
 in an insert (right) line | ## Development python3 -m venv venv source venv/
```

### Comparing `webdiff-1.0.0/webdiff.egg-info/SOURCES.txt` & `webdiff-1.0.1/webdiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

