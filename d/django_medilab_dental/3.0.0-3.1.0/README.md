# Comparing `tmp/django_medilab_dental-3.0.0.tar.gz` & `tmp/django_medilab_dental-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_medilab_dental-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_medilab_dental-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_medilab_dental-3.0.0.tar` & `django_medilab_dental-3.1.0.tar`

### file list

```diff
@@ -1,163 +1,164 @@
--rw-r--r--   0        0        0       66 2024-05-23 04:28:06.999222 django_medilab_dental-3.0.0/.gitattributes
--rw-r--r--   0        0        0       52 2024-05-23 04:29:26.293941 django_medilab_dental-3.0.0/.idea/.gitignore
--rw-r--r--   0        0        0      411 2024-05-23 04:29:25.772294 django_medilab_dental-3.0.0/.idea/django-medilab-dental.iml
--rw-r--r--   0        0        0      174 2024-05-23 04:29:26.203911 django_medilab_dental-3.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      433 2024-05-23 05:02:00.053461 django_medilab_dental-3.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      294 2024-05-23 04:29:26.198245 django_medilab_dental-3.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-05-23 04:29:26.211631 django_medilab_dental-3.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_medilab_dental-3.0.0/LICENSE
--rw-r--r--   0        0        0     4823 2024-05-24 00:36:45.615188 django_medilab_dental-3.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-23 05:01:44.415947 django_medilab_dental-3.0.0/django_medilab_dental/__init__.py
--rw-r--r--   0        0        0      351 2024-05-24 01:40:45.216255 django_medilab_dental-3.0.0/django_medilab_dental/admin.py
--rw-r--r--   0        0        0      172 2024-05-23 05:01:44.417576 django_medilab_dental-3.0.0/django_medilab_dental/apps.py
--rw-r--r--   0        0        0      921 2024-05-21 05:02:10.461971 django_medilab_dental-3.0.0/django_medilab_dental/forms.py
--rw-r--r--   0        0        0     1859 2024-05-24 01:41:10.406636 django_medilab_dental-3.0.0/django_medilab_dental/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-17 05:17:43.157727 django_medilab_dental-3.0.0/django_medilab_dental/migrations/__init__.py
--rw-r--r--   0        0        0     1606 2024-05-24 01:32:18.710158 django_medilab_dental-3.0.0/django_medilab_dental/models.py
--rw-r--r--   0        0        0      655 2024-05-24 01:40:45.218973 django_medilab_dental-3.0.0/django_medilab_dental/sitemaps.py
--rwxr-xr-x   0        0        0    30612 2024-05-21 00:40:32.551366 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/css/style.css
--rwxr-xr-x   0        0        0     5371 2024-03-17 05:37:08.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/js/main.js
--rwxr-xr-x   0        0        0     3160 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_footer.scss
--rwxr-xr-x   0        0        0     1769 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_general.scss
--rwxr-xr-x   0        0        0     1981 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_header.scss
--rwxr-xr-x   0        0        0     1424 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_hero.scss
--rwxr-xr-x   0        0        0     3911 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_nav.scss
--rwxr-xr-x   0        0        0    20291 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_sections.scss
--rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_variables.scss
--rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/style.scss
--rw-r--r--   0        0        0    70607 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.compat.css
--rw-r--r--   0        0        0    95374 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.css
--rwxr-xr-x   0        0        0    71750 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.min.css
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/animations.css
--rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.css
--rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.min.css
--rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/transformations.css
--rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.eot
--rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.svg
--rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.ttf
--rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff
--rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff2
--rw-r--r--   0        0        0   141265 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.css
--rw-r--r--   0        0        0   103009 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.min.css
--rw-r--r--   0        0        0    24920 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.css
--rw-r--r--   0        0        0    19582 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.min.css
--rw-r--r--   0        0        0   113480 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.css
--rw-r--r--   0        0        0    80888 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.min.css
--rw-r--r--   0        0        0      633 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.css
--rw-r--r--   0        0        0      580 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.min.css
--rw-r--r--   0        0        0      625 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.css
--rw-r--r--   0        0        0      572 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.min.css
--rw-r--r--   0        0        0    21696 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.css
--rw-r--r--   0        0        0    17011 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.min.css
--rw-r--r--   0        0        0     1831 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.css
--rw-r--r--   0        0        0     1736 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.min.css
--rw-r--r--   0        0        0    41574 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.css
--rw-r--r--   0        0        0    27593 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.min.css
--rw-r--r--   0        0        0      871 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.css
--rw-r--r--   0        0        0      794 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.min.css
--rw-r--r--   0        0        0   209128 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117852 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    67860 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25392 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   420332 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156400 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0   109600 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    56300 2024-04-07 13:11:34.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0     5417 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js
--rw-r--r--   0        0        0    24750 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js.map
--rw-r--r--   0        0        0   138761 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.css
--rw-r--r--   0        0        0   525744 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.eot
--rw-r--r--   0        0        0  3776084 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.glyph.json
--rw-r--r--   0        0        0   138773 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.less
--rw-r--r--   0        0        0  2460531 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.svg
--rw-r--r--   0        0        0  1582046 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.symbol.svg
--rw-r--r--   0        0        0   525572 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.ttf
--rw-r--r--   0        0        0   224116 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff
--rw-r--r--   0        0        0   163200 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff2
--rw-r--r--   0        0        0    18432 2024-04-20 04:09:20.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149982 2024-04-20 04:09:20.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   203001 2024-04-20 04:09:20.000000 django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     1085 2024-05-22 06:34:05.468294 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_about.html
--rw-r--r--   0        0        0     1201 2024-05-22 06:34:05.457467 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_appointment.html
--rw-r--r--   0        0        0     2369 2024-05-23 07:12:50.126310 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_contact.html
--rw-r--r--   0        0        0      481 2024-05-21 02:28:41.815055 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_counts.html
--rw-r--r--   0        0        0     1407 2024-05-22 06:34:05.464894 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_departments.html
--rw-r--r--   0        0        0     1397 2024-05-22 06:34:05.481019 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_doctors.html
--rw-r--r--   0        0        0     1009 2024-05-21 07:04:19.229553 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_faq.html
--rw-r--r--   0        0        0      705 2024-05-22 01:55:04.082872 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_gallery.html
--rw-r--r--   0        0        0      528 2024-05-22 06:34:05.461548 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_hero.html
--rw-r--r--   0        0        0      630 2024-05-21 05:04:08.067506 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_services.html
--rw-r--r--   0        0        0     1021 2024-05-22 06:34:05.473750 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_testimonials.html
--rw-r--r--   0        0        0     1198 2024-05-21 01:13:06.372770 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_why-us.html
--rwxr-xr-x   0        0        0      492 2024-05-24 01:40:45.228467 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/blog-details.html
--rw-r--r--   0        0        0      377 2024-05-24 01:40:45.213013 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/breadcrumb.html
--rw-r--r--   0        0        0     3070 2024-05-24 01:44:00.372775 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/footer.html
--rwxr-xr-x   0        0        0     1579 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/forms/appointment.php
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/forms/contact.php
--rw-r--r--   0        0        0     2780 2024-05-22 06:15:39.187054 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/header.html
--rwxr-xr-x   0        0        0     4117 2024-05-23 05:16:43.713476 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/index.html
--rwxr-xr-x   0        0        0    16287 2024-05-23 00:41:03.798823 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/privacy.html
--rw-r--r--   0        0        0     1935 2024-05-22 06:20:30.241173 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/seo.html
--rwxr-xr-x   0        0        0    16327 2024-05-23 00:41:03.804529 django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/terms.html
--rw-r--r--   0        0        0     5322 2024-05-24 01:40:45.208904 django_medilab_dental-3.0.0/django_medilab_dental/templatetags/medilabdental_tags.py
--rw-r--r--   0        0        0       60 2024-05-23 05:01:44.417841 django_medilab_dental-3.0.0/django_medilab_dental/tests.py
--rw-r--r--   0        0        0      802 2024-05-24 01:40:45.221206 django_medilab_dental-3.0.0/django_medilab_dental/urls.py
--rw-r--r--   0        0        0     4165 2024-05-24 01:40:45.226031 django_medilab_dental-3.0.0/django_medilab_dental/views.py
--rw-r--r--   0        0        0      973 2024-05-24 00:36:45.620110 django_medilab_dental-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 django_medilab_dental-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-05-24 02:02:32.196834 django_medilab_dental-3.1.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-05-23 04:28:06.999222 django_medilab_dental-3.1.0/.gitattributes
+-rw-r--r--   0        0        0       52 2024-05-23 04:29:26.293941 django_medilab_dental-3.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      411 2024-05-23 04:29:25.772294 django_medilab_dental-3.1.0/.idea/django-medilab-dental.iml
+-rw-r--r--   0        0        0      174 2024-05-23 04:29:26.203911 django_medilab_dental-3.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      433 2024-05-23 05:02:00.053461 django_medilab_dental-3.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2024-05-23 04:29:26.198245 django_medilab_dental-3.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-05-23 04:29:26.211631 django_medilab_dental-3.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_medilab_dental-3.1.0/LICENSE
+-rw-r--r--   0        0        0     4823 2024-05-24 00:36:45.615188 django_medilab_dental-3.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 05:01:44.415947 django_medilab_dental-3.1.0/django_medilab_dental/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-24 01:40:45.216255 django_medilab_dental-3.1.0/django_medilab_dental/admin.py
+-rw-r--r--   0        0        0      172 2024-05-23 05:01:44.417576 django_medilab_dental-3.1.0/django_medilab_dental/apps.py
+-rw-r--r--   0        0        0      921 2024-05-21 05:02:10.461971 django_medilab_dental-3.1.0/django_medilab_dental/forms.py
+-rw-r--r--   0        0        0     1859 2024-05-24 01:41:10.406636 django_medilab_dental-3.1.0/django_medilab_dental/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:17:43.157727 django_medilab_dental-3.1.0/django_medilab_dental/migrations/__init__.py
+-rw-r--r--   0        0        0     1606 2024-05-24 01:32:18.710158 django_medilab_dental-3.1.0/django_medilab_dental/models.py
+-rw-r--r--   0        0        0      655 2024-05-24 01:40:45.218973 django_medilab_dental-3.1.0/django_medilab_dental/sitemaps.py
+-rwxr-xr-x   0        0        0    30612 2024-05-21 00:40:32.551366 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/css/style.css
+-rwxr-xr-x   0        0        0     5371 2024-03-17 05:37:08.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/js/main.js
+-rwxr-xr-x   0        0        0     3160 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_footer.scss
+-rwxr-xr-x   0        0        0     1769 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_general.scss
+-rwxr-xr-x   0        0        0     1981 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_header.scss
+-rwxr-xr-x   0        0        0     1424 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_hero.scss
+-rwxr-xr-x   0        0        0     3911 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_nav.scss
+-rwxr-xr-x   0        0        0    20291 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_sections.scss
+-rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_variables.scss
+-rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/style.scss
+-rw-r--r--   0        0        0    70607 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.compat.css
+-rw-r--r--   0        0        0    95374 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.css
+-rwxr-xr-x   0        0        0    71750 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.min.css
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/animations.css
+-rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.css
+-rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.min.css
+-rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/transformations.css
+-rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.eot
+-rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.svg
+-rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.ttf
+-rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff
+-rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff2
+-rw-r--r--   0        0        0   141265 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.css
+-rw-r--r--   0        0        0   103009 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.min.css
+-rw-r--r--   0        0        0    24920 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.css
+-rw-r--r--   0        0        0    19582 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.min.css
+-rw-r--r--   0        0        0   113480 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.css
+-rw-r--r--   0        0        0    80888 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.min.css
+-rw-r--r--   0        0        0      633 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.css
+-rw-r--r--   0        0        0      580 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.min.css
+-rw-r--r--   0        0        0      625 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.css
+-rw-r--r--   0        0        0      572 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.min.css
+-rw-r--r--   0        0        0    21696 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.css
+-rw-r--r--   0        0        0    17011 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.min.css
+-rw-r--r--   0        0        0     1831 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.css
+-rw-r--r--   0        0        0     1736 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.min.css
+-rw-r--r--   0        0        0    41574 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.css
+-rw-r--r--   0        0        0    27593 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.min.css
+-rw-r--r--   0        0        0      871 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.css
+-rw-r--r--   0        0        0      794 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.min.css
+-rw-r--r--   0        0        0   209128 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117852 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    67860 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25392 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   420332 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156400 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0   109600 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    56300 2024-04-07 13:11:34.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0     5417 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js
+-rw-r--r--   0        0        0    24750 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js.map
+-rw-r--r--   0        0        0   138761 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.css
+-rw-r--r--   0        0        0   525744 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.eot
+-rw-r--r--   0        0        0  3776084 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.glyph.json
+-rw-r--r--   0        0        0   138773 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.less
+-rw-r--r--   0        0        0  2460531 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.svg
+-rw-r--r--   0        0        0  1582046 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.symbol.svg
+-rw-r--r--   0        0        0   525572 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.ttf
+-rw-r--r--   0        0        0   224116 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff
+-rw-r--r--   0        0        0   163200 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff2
+-rw-r--r--   0        0        0    18432 2024-04-20 04:09:20.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149982 2024-04-20 04:09:20.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   203001 2024-04-20 04:09:20.000000 django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     1136 2024-05-30 01:59:53.913278 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_about.html
+-rw-r--r--   0        0        0     1201 2024-05-22 06:34:05.457467 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_appointment.html
+-rw-r--r--   0        0        0     2369 2024-05-23 07:12:50.126310 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_contact.html
+-rw-r--r--   0        0        0      481 2024-05-21 02:28:41.815055 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_counts.html
+-rw-r--r--   0        0        0     1407 2024-05-22 06:34:05.464894 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_departments.html
+-rw-r--r--   0        0        0     1397 2024-05-22 06:34:05.481019 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_doctors.html
+-rw-r--r--   0        0        0     1009 2024-05-21 07:04:19.229553 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_faq.html
+-rw-r--r--   0        0        0      705 2024-05-22 01:55:04.082872 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_gallery.html
+-rw-r--r--   0        0        0      528 2024-05-22 06:34:05.461548 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_hero.html
+-rw-r--r--   0        0        0      630 2024-05-21 05:04:08.067506 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_services.html
+-rw-r--r--   0        0        0     1021 2024-05-22 06:34:05.473750 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_testimonials.html
+-rw-r--r--   0        0        0     1198 2024-05-21 01:13:06.372770 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_why-us.html
+-rwxr-xr-x   0        0        0      492 2024-05-24 01:40:45.228467 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/blog-details.html
+-rw-r--r--   0        0        0      377 2024-05-24 01:40:45.213013 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/breadcrumb.html
+-rw-r--r--   0        0        0     3070 2024-05-24 01:44:00.372775 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/footer.html
+-rwxr-xr-x   0        0        0     1579 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/forms/appointment.php
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/forms/contact.php
+-rw-r--r--   0        0        0     2780 2024-05-22 06:15:39.187054 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/header.html
+-rwxr-xr-x   0        0        0     4117 2024-05-23 05:16:43.713476 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/index.html
+-rwxr-xr-x   0        0        0    16287 2024-05-23 00:41:03.798823 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/privacy.html
+-rw-r--r--   0        0        0     1935 2024-05-22 06:20:30.241173 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/seo.html
+-rwxr-xr-x   0        0        0    16327 2024-05-23 00:41:03.804529 django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/terms.html
+-rw-r--r--   0        0        0     5322 2024-05-24 01:40:45.208904 django_medilab_dental-3.1.0/django_medilab_dental/templatetags/medilabdental_tags.py
+-rw-r--r--   0        0        0       60 2024-05-23 05:01:44.417841 django_medilab_dental-3.1.0/django_medilab_dental/tests.py
+-rw-r--r--   0        0        0      802 2024-05-24 01:40:45.221206 django_medilab_dental-3.1.0/django_medilab_dental/urls.py
+-rw-r--r--   0        0        0     4165 2024-05-24 01:40:45.226031 django_medilab_dental-3.1.0/django_medilab_dental/views.py
+-rw-r--r--   0        0        0      973 2024-05-30 02:03:27.759459 django_medilab_dental-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5563 1970-01-01 00:00:00.000000 django_medilab_dental-3.1.0/PKG-INFO
```

### Comparing `django_medilab_dental-3.0.0/LICENSE` & `django_medilab_dental-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/README.md` & `django_medilab_dental-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/forms.py` & `django_medilab_dental-3.1.0/django_medilab_dental/forms.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/migrations/0001_initial.py` & `django_medilab_dental-3.1.0/django_medilab_dental/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/models.py` & `django_medilab_dental-3.1.0/django_medilab_dental/models.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/sitemaps.py` & `django_medilab_dental-3.1.0/django_medilab_dental/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/css/style.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/css/style.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/js/main.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/js/main.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_footer.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_general.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_header.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_hero.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_nav.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/scss/_sections.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.compat.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.compat.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/animate.css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.json` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/animations.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/transformations.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.eot` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.svg` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.ttf` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/css/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.min.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/php-email-form.php` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/validate.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/purecounter/purecounter_vanilla.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.eot` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.eot`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.glyph.json` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.glyph.json`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.less` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.less`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.svg` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.svg`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.symbol.svg` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.symbol.svg`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.ttf` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff2` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/remixicon/remixicon.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.css` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js.map` & `django_medilab_dental-3.1.0/django_medilab_dental/static/medilabdental/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_about.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_about.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,22 @@
   }
 </style>
 
 <section id="about" class="about">
   <div class="container-fluid">
 
     <div class="row">
+
       <div class="col-xl-5 col-lg-6 video-box d-flex justify-content-center align-items-stretch position-relative">
+        {% if about_video %}
         <a href="{{ about_video }}" class="glightbox play-btn mb-4"></a>
+        {% endif %}
       </div>
 
+
       <div class="col-xl-7 col-lg-6 icon-boxes d-flex flex-column align-items-stretch justify-content-center py-5 px-lg-5">
         {% autoescape off%}
         <h3>{{ about_h3 }}</h3>
         <p>{{ about_p }}</p>
         {% endautoescape %}
 
         {% for item in about %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 {% load static %}
+{% if about_video %} {% endif %}
 {% autoescape off%}
 ******** {{{{ aabboouutt__hh33 }}}} ********
 {{ about_p }}
 {% endautoescape %} {% for item in about %}
 ****** _{{_{{_ _ii_tt_ee_mm_.._hh_44_ _}}_}} ******
 {{ item.p }}
 {% endfor %}
```

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_appointment.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_appointment.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_contact.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_contact.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_departments.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_departments.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_doctors.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_doctors.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_faq.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_faq.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_gallery.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_gallery.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_hero.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_hero.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_services.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_services.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_testimonials.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/_why-us.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/_why-us.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/footer.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/footer.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/forms/appointment.php` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/forms/appointment.php`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/forms/contact.php` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/header.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/header.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/index.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/index.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/privacy.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/privacy.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/seo.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/seo.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templates/medilabdental/terms.html` & `django_medilab_dental-3.1.0/django_medilab_dental/templates/medilabdental/terms.html`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/templatetags/medilabdental_tags.py` & `django_medilab_dental-3.1.0/django_medilab_dental/templatetags/medilabdental_tags.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/urls.py` & `django_medilab_dental-3.1.0/django_medilab_dental/urls.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/django_medilab_dental/views.py` & `django_medilab_dental-3.1.0/django_medilab_dental/views.py`

 * *Files identical despite different names*

### Comparing `django_medilab_dental-3.0.0/pyproject.toml` & `django_medilab_dental-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_medilab_dental"
-version = "3.0.0"
+version = "3.1.0"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_medilab_dental-3.0.0/PKG-INFO` & `django_medilab_dental-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_medilab_dental
-Version: 3.0.0
+Version: 3.1.0
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
```

