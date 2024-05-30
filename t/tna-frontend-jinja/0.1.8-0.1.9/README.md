# Comparing `tmp/tna-frontend-jinja-0.1.8.tar.gz` & `tmp/tna-frontend-jinja-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tna-frontend-jinja-0.1.8.tar", last modified: Thu Dec 14 15:31:15 2023, max compression
+gzip compressed data, was "tna-frontend-jinja-0.1.9.tar", last modified: Fri Dec 29 12:19:47 2023, max compression
```

## Comparing `tna-frontend-jinja-0.1.8.tar` & `tna-frontend-jinja-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.072745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.072745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.072745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/breadcrumbs/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/breadcrumbs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/button/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/button/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/card/
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/card/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/checkboxes/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/checkboxes/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/cookie-banner/
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/cookie-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/date-input/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/date-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/date-search/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/date-search/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/featured-records/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/featured-records/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/filters/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/footer/
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/footer/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/grid/
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/grid/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/header/
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/header/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/hero/
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/hero/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/index-grid/
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/index-grid/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/message/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/message/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/pagination/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.076745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/phase-banner/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/phase-banner/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/picture/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/picture/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/radios/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/radios/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/search-field/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/search-field/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/select/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/select/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/sensitive-image/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/sensitive-image/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/skip-link/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/skip-link/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/tabs/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/text-input/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/text-input/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/textarea/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/textarea/macro.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2023-12-14 15:31:04.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 15:31:15.080745 tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2023-12-14 15:31:15.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-14 15:31:15.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 15:31:15.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-14 15:31:15.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-14 15:31:15.000000 tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.680827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.680827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/breadcrumbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/breadcrumbs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/button/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/card/
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/card/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/checkboxes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/checkboxes/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/cookie-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/cookie-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/date-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/date-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/date-search/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/date-search/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/featured-records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/featured-records/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/filters/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/footer/
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/footer/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/grid/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/header/
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/header/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/hero/
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/hero/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/index-grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/index-grid/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.684826 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/message/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/pagination/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/phase-banner/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/phase-banner/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/picture/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/picture/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/radios/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/radios/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/search-field/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/search-field/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/select/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/select/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/sensitive-image/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/sensitive-image/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/skip-link/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/skip-link/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/tabs/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/text-input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/text-input/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/textarea/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/textarea/macro.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2023-12-29 12:19:35.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 12:19:47.688827 tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2023-12-29 12:19:47.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-29 12:19:47.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 12:19:47.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-29 12:19:47.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-29 12:19:47.000000 tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/top_level.txt
```

### Comparing `tna-frontend-jinja-0.1.8/PKG-INFO` & `tna-frontend-jinja-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tna-frontend-jinja
-Version: 0.1.8
+Version: 0.1.9
 Summary: TNA Frontend Jinja templates
 Home-page: https://github.com/nationalarchives/tna-frontend-jinja
 Author: Andrew Hosgood
 Author-email: andrew.hosgood@nationalarchives.gov.uk
 Project-URL: Bug Tracker, https://github.com/nationalarchives/tna-frontend-jinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -66,18 +66,20 @@
 
 The included templates are a like-for-like port, the only difference between the Nunjucks examples and their Jinja equivalents is having to quote key names, e.g. `'text'` instead of `text`.
 
 We test each component against its published [component fixtures](https://github.com/nationalarchives/tna-frontend/blob/main/src/nationalarchives/components/button/fixtures.json) to ensure complete compatibility.
 
 ## Compatibility with TNA Frontend
 
-| TNA Frontend Jinja    | TNA Frontend                               |
+| TNA Frontend Jinja    | Compatible TNA Frontend versions           |
 | --------------------- | ------------------------------------------ |
-| `0.1.7`&ndash;`0.1.8` | `v0.1.31`                                  |
-| `0.1.6`               | `v0.1.29-prerelease`&ndash;`v0.1.30`       |
+| `0.1.9`               | `v0.1.33`                                  |
+| `0.1.8`               | `v0.1.31`, `v0.1.32`                       |
+| `0.1.7`               | `v0.1.31`, `v0.1.32`                       |
+| `0.1.6`               | `v0.1.29-prerelease`, `v0.1.30`            |
 | `0.1.0`&ndash;`0.1.5` | [latest from `main` branch when published] |
 
 ## Test the templates
 
 ```sh
 python -m venv venv
 python install -r test/requirements.txt
```

### Comparing `tna-frontend-jinja-0.1.8/README.md` & `tna-frontend-jinja-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,20 @@
 
 The included templates are a like-for-like port, the only difference between the Nunjucks examples and their Jinja equivalents is having to quote key names, e.g. `'text'` instead of `text`.
 
 We test each component against its published [component fixtures](https://github.com/nationalarchives/tna-frontend/blob/main/src/nationalarchives/components/button/fixtures.json) to ensure complete compatibility.
 
 ## Compatibility with TNA Frontend
 
-| TNA Frontend Jinja    | TNA Frontend                               |
+| TNA Frontend Jinja    | Compatible TNA Frontend versions           |
 | --------------------- | ------------------------------------------ |
-| `0.1.7`&ndash;`0.1.8` | `v0.1.31`                                  |
-| `0.1.6`               | `v0.1.29-prerelease`&ndash;`v0.1.30`       |
+| `0.1.9`               | `v0.1.33`                                  |
+| `0.1.8`               | `v0.1.31`, `v0.1.32`                       |
+| `0.1.7`               | `v0.1.31`, `v0.1.32`                       |
+| `0.1.6`               | `v0.1.29-prerelease`, `v0.1.30`            |
 | `0.1.0`&ndash;`0.1.5` | [latest from `main` branch when published] |
 
 ## Test the templates
 
 ```sh
 python -m venv venv
 python install -r test/requirements.txt
```

### Comparing `tna-frontend-jinja-0.1.8/setup.py` & `tna-frontend-jinja-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tna-frontend-jinja",
-    version="0.1.8",
+    version="0.1.9",
     author="Andrew Hosgood",
     author_email="andrew.hosgood@nationalarchives.gov.uk",
     description="TNA Frontend Jinja templates",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nationalarchives/tna-frontend-jinja",
     project_urls={
```

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/breadcrumbs/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/breadcrumbs/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/button/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/button/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/card/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/card/macro.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% macro tnaCard(params) %}
 {%- set htmlElement = params.htmlElement if params.htmlElement else 'div' -%}
 {%- set containerClasses = [params.classes] if params.classes else [] -%}
 {%- if params.horizontal -%}
   {%- set containerClasses = containerClasses + ['tna-card--horizontal'] -%}
 {%- endif -%}
-{%- if params.style == "boxed" -%}
+{%- if params.style == "contrast" -%}
   {%- set containerClasses = containerClasses + ['tna-card--contrast'] -%}
 {%- elif params.style == "accent" -%}
   {%- set containerClasses = containerClasses + ['tna-card--accent'] -%}
 {%- endif -%}
 {%- set classes = ' '.join(containerClasses) -%}
 <{{ htmlElement }} class="tna-card{% if classes %} {{ classes }}{% endif %}" {%- if params.attributes %}{% for attribute, value in params.attributes.items() %} {{ attribute }}="{{ value }}"{% endfor %}{% endif %}>
   <div class="tna-card__inner">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% macro tnaCard(params) %} {%- set htmlElement = params.htmlElement if
 params.htmlElement else 'div' -%} {%- set containerClasses = [params.classes]
 if params.classes else [] -%} {%- if params.horizontal -%} {%- set
 containerClasses = containerClasses + ['tna-card--horizontal'] -%} {%- endif -
-%} {%- if params.style == "boxed" -%} {%- set containerClasses =
+%} {%- if params.style == "contrast" -%} {%- set containerClasses =
 containerClasses + ['tna-card--contrast'] -%} {%- elif params.style == "accent"
 -%} {%- set containerClasses = containerClasses + ['tna-card--accent'] -%} {%-
 endif -%} {%- set classes = ' '.join(containerClasses) -%} <{{ htmlElement }}
 class="tna-card{% if classes %} {{ classes }}{% endif %}" {%- if
 params.attributes %}{% for attribute, value in params.attributes.items() %} {
 { attribute }}="{{ value }}"{% endfor %}{% endif %}>
 {%- if params.supertitle %}
```

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/checkboxes/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/checkboxes/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/cookie-banner/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/cookie-banner/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/date-input/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/date-input/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/date-search/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/date-search/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/featured-records/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/featured-records/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/filters/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/filters/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/footer/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/footer/macro.html`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,19 @@
         <li class="tna-footer__legal-item">
           <a href="{{ item.href }}" class="tna-footer__legal-item-link" {%- if item.title %} title="{{ item.title }}"{% endif %}>
             {{ item.text }}
           </a>
         </li>
         {%- endfor -%}
       </ul>
-      <hr />
+      <hr>
     </nav>
     {%- else -%}
     <div class="tna-column--full">
-      <hr />
+      <hr>
     </div>
     {%- endif -%}
   </div>
   <div class="tna-container tna-footer__licence">
     <div class="tna-column tna-column--full-tiny">
       <svg class="tna-footer__licence-logo" xmlns="http://www.w3.org/2000/svg" focusable="false" aria-hidden="true" viewBox="0 0 483.2 195.7" width="60" height="24">
         <path fill="currentColor" d="M421.5 142.8V.1l-50.7 32.3v161.1h112.4v-50.7zm-122.3-9.6A47.12 47.12 0 0 1 221 97.8c0-26 21.1-47.1 47.1-47.1 16.7 0 31.4 8.7 39.7 21.8l42.7-27.2A97.63 97.63 0 0 0 268.1 0c-36.5 0-68.3 20.1-85.1 49.7A98 98 0 0 0 97.8 0C43.9 0 0 43.9 0 97.8s43.9 97.8 97.8 97.8c36.5 0 68.3-20.1 85.1-49.7a97.76 97.76 0 0 0 149.6 25.4l19.4 22.2h3v-87.8h-80l24.3 27.5zM97.8 145c-26 0-47.1-21.1-47.1-47.1s21.1-47.1 47.1-47.1 47.2 21 47.2 47S123.8 145 97.8 145"></path>
```

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/grid/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/grid/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/header/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/header/macro.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   {%- set containerClasses = containerClasses + ['tna-header--accent'] -%}
 {%- endif -%}
 <header class="tna-header {{ ' '.join(containerClasses) }}" data-module="tna-header"{% for attribute, value in params.attributes %} {{ attribute }}="{{ value }}"{% endfor %}>
   {%- if params.exit -%}
   <div class="tna-header__exit">
     <div class="tna-container">
       <div class="tna-column tna-column--full">
-        <a href="{{ params.exit.href }}" class="tna-header__exit-link"{%- if params.exit.target %} target="{{ params.exit.target }}"{%- endif -%}>
+        <a href="{{ params.exit.href }}" class="tna-header__exit-link"{%- if params.exit.target %} target="{{ params.exit.target }}"{% endif %}>
           {{ params.exit.text }}
           {%- if params.exit.target == "_blank" -%}
           <i class="fa-solid fa-arrow-up-right-from-square"></i>
           {%- endif -%}
         </a>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% macro tnaHeader(params) %} {%- set containerClasses = [params.classes] if
 params.classes else [] -%} {%- if params.accent -%} {%- set containerClasses =
 containerClasses + ['tna-header--accent'] -%} {%- endif -%}
 % for attribute, value in params.attributes %} {{ attribute }}="{{ value }}"{%
 endfor %}> {%- if params.exit -%}
-%- if params.exit.target %} target="{{ params.exit.target }}"{%- endif -%}> {
+%- if params.exit.target %} target="{{ params.exit.target }}"{% endif %}> {
 { params.exit.text }} {%- if params.exit.target == "_blank" -%} {%- endif -%}
 {%- endif -%}
 <{%- if params.logo.href -%}a href="{{ params.logo.href }}" class="tna-
 header__logo-link tna-header__logo-link--href" title="{%- if params.logo.title
 -%}{{ params.logo.title }}{%- else -%}The National Archives{%- if
 params.logo.strapline %} - {{ params.logo.strapline }}{%- endif -%}{%- endif -
 %}"{%- else -%}span class="tna-header__logo-link"{%- endif -%}> {%- if
```

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/hero/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/hero/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/index-grid/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/index-grid/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/message/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/message/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/pagination/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/pagination/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/phase-banner/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/phase-banner/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/picture/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/picture/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/radios/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/radios/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/search-field/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/search-field/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/select/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/select/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/sensitive-image/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/sensitive-image/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/tabs/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/tabs/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/text-input/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/text-input/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/components/textarea/macro.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/components/textarea/macro.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja/templates/layouts/base.html` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/PKG-INFO` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tna-frontend-jinja
-Version: 0.1.8
+Version: 0.1.9
 Summary: TNA Frontend Jinja templates
 Home-page: https://github.com/nationalarchives/tna-frontend-jinja
 Author: Andrew Hosgood
 Author-email: andrew.hosgood@nationalarchives.gov.uk
 Project-URL: Bug Tracker, https://github.com/nationalarchives/tna-frontend-jinja/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -66,18 +66,20 @@
 
 The included templates are a like-for-like port, the only difference between the Nunjucks examples and their Jinja equivalents is having to quote key names, e.g. `'text'` instead of `text`.
 
 We test each component against its published [component fixtures](https://github.com/nationalarchives/tna-frontend/blob/main/src/nationalarchives/components/button/fixtures.json) to ensure complete compatibility.
 
 ## Compatibility with TNA Frontend
 
-| TNA Frontend Jinja    | TNA Frontend                               |
+| TNA Frontend Jinja    | Compatible TNA Frontend versions           |
 | --------------------- | ------------------------------------------ |
-| `0.1.7`&ndash;`0.1.8` | `v0.1.31`                                  |
-| `0.1.6`               | `v0.1.29-prerelease`&ndash;`v0.1.30`       |
+| `0.1.9`               | `v0.1.33`                                  |
+| `0.1.8`               | `v0.1.31`, `v0.1.32`                       |
+| `0.1.7`               | `v0.1.31`, `v0.1.32`                       |
+| `0.1.6`               | `v0.1.29-prerelease`, `v0.1.30`            |
 | `0.1.0`&ndash;`0.1.5` | [latest from `main` branch when published] |
 
 ## Test the templates
 
 ```sh
 python -m venv venv
 python install -r test/requirements.txt
```

### Comparing `tna-frontend-jinja-0.1.8/tna_frontend_jinja.egg-info/SOURCES.txt` & `tna-frontend-jinja-0.1.9/tna_frontend_jinja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

