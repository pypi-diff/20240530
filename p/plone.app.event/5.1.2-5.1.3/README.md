# Comparing `tmp/plone.app.event-5.1.2.tar.gz` & `tmp/plone_app_event-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.event-5.1.2.tar", last modified: Tue Apr 16 19:33:06 2024, max compression
+gzip compressed data, was "plone_app_event-5.1.3.tar", last modified: Thu May 30 18:35:35 2024, max compression
```

## Comparing `plone.app.event-5.1.2.tar` & `plone_app_event-5.1.3.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.222715 plone.app.event-5.1.2/
--rw-r--r--   0 maurits    (501) staff       (20)    58418 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)    18099 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      756 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      202 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    64112 2024-04-16 19:33:06.222303 plone.app.event-5.1.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      587 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.187437 plone.app.event-5.1.2/docs/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.188774 plone.app.event-5.1.2/docs/api/
--rw-r--r--   0 maurits    (501) staff       (20)       94 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/base.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.190353 plone.app.event-5.1.2/docs/api/browser/
--rw-r--r--   0 maurits    (501) staff       (20)      145 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/event_listing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      146 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/event_summary.rst
--rw-r--r--   0 maurits    (501) staff       (20)      136 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/event_view.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/formatted_date.rst
--rw-r--r--   0 maurits    (501) staff       (20)      158 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/browser/leadimage_viewlet.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.191279 plone.app.event-5.1.2/docs/api/dx/
--rw-r--r--   0 maurits    (501) staff       (20)      118 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/dx/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/dx/interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)      119 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/dx/traverser.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.191889 plone.app.event-5.1.2/docs/api/ical/
--rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/ical/exporter.rst
--rw-r--r--   0 maurits    (501) staff       (20)      121 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/ical/importer.rst
--rw-r--r--   0 maurits    (501) staff       (20)      403 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      112 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)      113 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/api/recurrence.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5633 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/architectural-overview.rst
--rw-r--r--   0 maurits    (501) staff       (20)      395 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)     3464 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/designchoices.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10346 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/development.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1589 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2839 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/installation.rst
--rw-r--r--   0 maurits    (501) staff       (20)      884 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/docs/tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.192173 plone.app.event-5.1.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.194783 plone.app.event-5.1.2/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.197856 plone.app.event-5.1.2/plone/app/event/
--rw-r--r--   0 maurits    (501) staff       (20)      369 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    33259 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/base.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.202027 plone.app.event-5.1.2/plone/app/event/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3398 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5435 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15434 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     9719 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_summary.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2965 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      605 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/event_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3228 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/formatted_date.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1001 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/formatted_date.py
--rw-r--r--   0 maurits    (501) staff       (20)      726 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/formatted_start_date.pt
--rw-r--r--   0 maurits    (501) staff       (20)      550 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/leadimage_viewlet.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.202585 plone.app.event-5.1.2/plone/app/event/browser/resources/
--rw-r--r--   0 maurits    (501) staff       (20)      349 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/resources/calendar.svg
--rw-r--r--   0 maurits    (501) staff       (20)     3726 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/browser/resources/event.js
--rw-r--r--   0 maurits    (501) staff       (20)     2121 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.204358 plone.app.event-5.1.2/plone/app/event/dx/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    14485 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1981 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      585 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/ical.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/dx/traverser.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.205649 plone.app.event-5.1.2/plone/app/event/ical/
--rw-r--r--   0 maurits    (501) staff       (20)      430 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3135 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    14653 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/exporter.py
--rw-r--r--   0 maurits    (501) staff       (20)    14459 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/ical/importer.py
--rw-r--r--   0 maurits    (501) staff       (20)      350 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      171 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.207483 plone.app.event-5.1.2/plone/app/event/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)      767 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      836 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4035 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.pt
--rw-r--r--   0 maurits    (501) staff       (20)    11194 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)     3357 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9912 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.180886 plone.app.event-5.1.2/plone/app/event/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.210110 plone.app.event-5.1.2/plone/app/event/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     2651 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      157 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      357 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      321 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/plone.app.event-default.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1194 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      479 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      328 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.211363 plone.app.event-5.1.2/plone/app/event/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)      190 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types/Collection.xml
--rw-r--r--   0 maurits    (501) staff       (20)      186 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 maurits    (501) staff       (20)      355 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.211947 plone.app.event-5.1.2/plone/app/event/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      181 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.212284 plone.app.event-5.1.2/plone/app/event/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2850 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
--rw-r--r--   0 maurits    (501) staff       (20)      199 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     6714 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)      567 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/recurrence.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2462 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     3694 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.217607 plone.app.event-5.1.2/plone/app/event/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      898 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/INACTIVE_test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5841 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/base_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     2201 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/icaltest.ics
--rw-r--r--   0 maurits    (501) staff       (20)     2202 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/icaltest2.ics
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.218341 plone.app.event-5.1.2/plone/app/event/tests/javascripts/
--rw-r--r--   0 maurits    (501) staff       (20)    23860 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.html
--rw-r--r--   0 maurits    (501) staff       (20)      715 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.218957 plone.app.event-5.1.2/plone/app/event/tests/qunit/
--rw-r--r--   0 maurits    (501) staff       (20)     3952 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.css
--rw-r--r--   0 maurits    (501) staff       (20)    37060 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.js
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.219853 plone.app.event-5.1.2/plone/app/event/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     6114 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/robot/test_event_roundtrip.robot
--rw-r--r--   0 maurits    (501) staff       (20)      633 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/robot/variables.py
--rw-r--r--   0 maurits    (501) staff       (20)    35328 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_base_module.py
--rw-r--r--   0 maurits    (501) staff       (20)      773 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)    22404 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_dx_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     6395 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_event_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     4982 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_event_summary.py
--rw-r--r--   0 maurits    (501) staff       (20)     2075 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_event_view.py
--rw-r--r--   0 maurits    (501) staff       (20)     3585 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_ical_import.py
--rw-r--r--   0 maurits    (501) staff       (20)    19302 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_icalendar.py
--rw-r--r--   0 maurits    (501) staff       (20)    10307 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_portlet_calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)    11112 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_portlet_events.py
--rw-r--r--   0 maurits    (501) staff       (20)    13916 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_recurrence.py
--rw-r--r--   0 maurits    (501) staff       (20)      544 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/tests/test_search.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.220781 plone.app.event-5.1.2/plone/app/event/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      969 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3415 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/upgrades/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)     1261 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/plone/app/event/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:33:06.221154 plone.app.event-5.1.2/plone.app.event.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    64112 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4236 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      710 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:33:06.000000 plone.app.event-5.1.2/plone.app.event.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4300 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-16 19:33:06.222792 plone.app.event-5.1.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2613 2024-04-16 19:33:05.000000 plone.app.event-5.1.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.633447 plone_app_event-5.1.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    58540 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18099 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      756 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    64234 2024-05-30 18:35:35.632664 plone_app_event-5.1.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      587 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.579164 plone_app_event-5.1.3/docs/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.581053 plone_app_event-5.1.3/docs/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/base.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.583466 plone_app_event-5.1.3/docs/api/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/browser/event_listing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/browser/event_summary.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      136 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/browser/event_view.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/browser/formatted_date.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      158 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/browser/leadimage_viewlet.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.584906 plone_app_event-5.1.3/docs/api/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)      118 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/dx/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/dx/interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      119 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/dx/traverser.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.585881 plone_app_event-5.1.3/docs/api/ical/
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/ical/exporter.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/ical/importer.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      112 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      113 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/api/recurrence.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5633 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/architectural-overview.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3464 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/designchoices.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10346 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/development.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1589 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2839 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/installation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      884 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/docs/tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.586352 plone_app_event-5.1.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.590313 plone_app_event-5.1.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.595108 plone_app_event-5.1.3/plone/app/event/
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    33259 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.600905 plone_app_event-5.1.3/plone/app/event/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3398 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5435 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/event_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    15434 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/event_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9719 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/event_summary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2965 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/event_summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/event_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      605 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/event_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3228 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/formatted_date.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1001 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/formatted_date.py
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/formatted_start_date.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/leadimage_viewlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.601840 plone_app_event-5.1.3/plone/app/event/browser/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)      349 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/resources/calendar.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     3726 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/browser/resources/event.js
+-rw-r--r--   0 maurits    (501) staff       (20)     2282 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.604781 plone_app_event-5.1.3/plone/app/event/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/dx/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14485 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/dx/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1981 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/dx/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/dx/ical.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/dx/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/dx/traverser.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.606850 plone_app_event-5.1.3/plone/app/event/ical/
+-rw-r--r--   0 maurits    (501) staff       (20)      430 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/ical/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3135 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/ical/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    14653 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/ical/exporter.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14459 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/ical/importer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      350 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      171 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.609902 plone_app_event-5.1.3/plone/app/event/portlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/portlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      836 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/portlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4035 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/portlets/portlet_calendar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11194 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/portlets/portlet_calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3357 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/portlets/portlet_events.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9912 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/portlets/portlet_events.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.570140 plone_app_event-5.1.3/plone/app/event/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.614171 plone_app_event-5.1.3/plone/app/event/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     2651 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      321 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/plone.app.event-default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1194 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      479 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      328 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.615646 plone_app_event-5.1.3/plone/app/event/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      355 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.616611 plone_app_event-5.1.3/plone/app/event/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      181 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.617155 plone_app_event-5.1.3/plone/app/event/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2850 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     6714 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      567 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/recurrence.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2462 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3694 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.625799 plone_app_event-5.1.3/plone/app/event/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      898 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/INACTIVE_test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5841 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/base_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2201 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/icaltest.ics
+-rw-r--r--   0 maurits    (501) staff       (20)     2202 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/icaltest2.ics
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.626826 plone_app_event-5.1.3/plone/app/event/tests/javascripts/
+-rw-r--r--   0 maurits    (501) staff       (20)    23860 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/javascripts/test_event.html
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/javascripts/test_event.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.627751 plone_app_event-5.1.3/plone/app/event/tests/qunit/
+-rw-r--r--   0 maurits    (501) staff       (20)     3952 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/qunit/qunit.css
+-rw-r--r--   0 maurits    (501) staff       (20)    37060 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/qunit/qunit.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.628837 plone_app_event-5.1.3/plone/app/event/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     6114 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/robot/test_event_roundtrip.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      633 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35328 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_base_module.py
+-rw-r--r--   0 maurits    (501) staff       (20)      773 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22404 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_dx_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6395 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_event_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4982 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_event_summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2075 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_event_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3585 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_ical_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19302 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_icalendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10307 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_portlet_calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11112 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_portlet_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13916 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      544 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/tests/test_search.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.630124 plone_app_event-5.1.3/plone/app/event/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      969 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3415 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/upgrades/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1261 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/plone/app/event/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-05-30 18:35:35.630722 plone_app_event-5.1.3/plone.app.event.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    64234 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4236 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      710 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-05-30 18:35:35.000000 plone_app_event-5.1.3/plone.app.event.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4300 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-05-30 18:35:35.633597 plone_app_event-5.1.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2613 2024-05-30 18:35:34.000000 plone_app_event-5.1.3/setup.py
```

### Comparing `plone.app.event-5.1.2/CHANGES.rst` & `plone_app_event-5.1.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.3 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Conditionally load the zcml for our portlets.
+  [maurits] (#3923)
+
+
 5.1.2 (2024-04-16)
 ------------------
 
 Bug fixes:
 
 
 - Fix calculation of eventaccessor urls @1letter (#387)
```

### Comparing `plone.app.event-5.1.2/LICENSE.GPL` & `plone_app_event-5.1.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/LICENSE.rst` & `plone_app_event-5.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/PKG-INFO` & `plone_app_event-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.1.2
+Version: 5.1.3
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -155,14 +155,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.3 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Conditionally load the zcml for our portlets.
+  [maurits] (#3923)
+
+
 5.1.2 (2024-04-16)
 ------------------
 
 Bug fixes:
 
 
 - Fix calculation of eventaccessor urls @1letter (#387)
```

### Comparing `plone.app.event-5.1.2/README.rst` & `plone_app_event-5.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/docs/architectural-overview.rst` & `plone_app_event-5.1.3/docs/architectural-overview.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/docs/designchoices.rst` & `plone_app_event-5.1.3/docs/designchoices.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/docs/development.rst` & `plone_app_event-5.1.3/docs/development.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/docs/index.rst` & `plone_app_event-5.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/docs/installation.rst` & `plone_app_event-5.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/docs/tests.rst` & `plone_app_event-5.1.3/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/base.py` & `plone_app_event-5.1.3/plone/app/event/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/configure.zcml` & `plone_app_event-5.1.3/plone/app/event/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/event_listing.pt` & `plone_app_event-5.1.3/plone/app/event/browser/event_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/event_listing.py` & `plone_app_event-5.1.3/plone/app/event/browser/event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/event_summary.pt` & `plone_app_event-5.1.3/plone/app/event/browser/event_summary.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/event_summary.py` & `plone_app_event-5.1.3/plone/app/event/browser/event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/event_view.pt` & `plone_app_event-5.1.3/plone/app/event/browser/event_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/event_view.py` & `plone_app_event-5.1.3/plone/app/event/browser/event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/formatted_date.pt` & `plone_app_event-5.1.3/plone/app/event/browser/formatted_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/formatted_date.py` & `plone_app_event-5.1.3/plone/app/event/browser/formatted_date.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/formatted_start_date.pt` & `plone_app_event-5.1.3/plone/app/event/browser/formatted_start_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/leadimage_viewlet.py` & `plone_app_event-5.1.3/plone/app/event/browser/leadimage_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/browser/resources/event.js` & `plone_app_event-5.1.3/plone/app/event/browser/resources/event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/configure.zcml` & `plone_app_event-5.1.3/plone/app/event/configure.zcml`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,31 @@
     >
 
   <!-- external dependencies -->
   <include package="plone.browserlayer" />
   <include package="plone.event" />
   <include package="plone.resource" />
   <include package="plone.formwidget.recurrence" />
-  <include package="plone.app.portlets" />
   <include package="plone.app.registry" />
   <include package="plone.app.z3cform" />
 
   <!-- internal dependencies -->
   <include file="permissions.zcml" />
   <include package=".dx" />
   <include package=".browser" />
-  <include package=".portlets" />
   <include package=".ical" />
   <include file="recurrence.zcml" />
   <include package=".upgrades" />
 
+  <configure zcml:condition="not-have disable-classic-ui">
+    <configure zcml:condition="installed plone.app.portlets">
+      <include package="plone.app.portlets" />
+      <include package=".portlets" />
+    </configure>
+  </configure>
   <utility
       name="plone.app.event.SynchronizationStrategies"
       component=".vocabularies.SynchronizationStrategies"
       />
 
   <genericsetup:registerProfile
       name="default"
```

### Comparing `plone.app.event-5.1.2/plone/app/event/dx/behaviors.py` & `plone_app_event-5.1.3/plone/app/event/dx/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/dx/configure.zcml` & `plone_app_event-5.1.3/plone/app/event/dx/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/dx/ical.zcml` & `plone_app_event-5.1.3/plone/app/event/dx/ical.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/dx/traverser.py` & `plone_app_event-5.1.3/plone/app/event/dx/traverser.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/ical/configure.zcml` & `plone_app_event-5.1.3/plone/app/event/ical/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/ical/exporter.py` & `plone_app_event-5.1.3/plone/app/event/ical/exporter.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/ical/importer.py` & `plone_app_event-5.1.3/plone/app/event/ical/importer.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/portlets/__init__.py` & `plone_app_event-5.1.3/plone/app/event/portlets/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/portlets/configure.zcml` & `plone_app_event-5.1.3/plone/app/event/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.pt` & `plone_app_event-5.1.3/plone/app/event/portlets/portlet_calendar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/portlets/portlet_calendar.py` & `plone_app_event-5.1.3/plone/app/event/portlets/portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.pt` & `plone_app_event-5.1.3/plone/app/event/portlets/portlet_events.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/portlets/portlet_events.py` & `plone_app_event-5.1.3/plone/app/event/portlets/portlet_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/profiles/default/actions.xml` & `plone_app_event-5.1.3/plone/app/event/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/profiles/default/portlets.xml` & `plone_app_event-5.1.3/plone/app/event/profiles/default/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml` & `plone_app_event-5.1.3/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/recurrence.py` & `plone_app_event-5.1.3/plone/app/event/recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/recurrence.zcml` & `plone_app_event-5.1.3/plone/app/event/recurrence.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/setuphandlers.py` & `plone_app_event-5.1.3/plone/app/event/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/testing.py` & `plone_app_event-5.1.3/plone/app/event/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/INACTIVE_test_robot.py` & `plone_app_event-5.1.3/plone/app/event/tests/INACTIVE_test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/base_setup.py` & `plone_app_event-5.1.3/plone/app/event/tests/base_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/icaltest.ics` & `plone_app_event-5.1.3/plone/app/event/tests/icaltest.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/icaltest2.ics` & `plone_app_event-5.1.3/plone/app/event/tests/icaltest2.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.html` & `plone_app_event-5.1.3/plone/app/event/tests/javascripts/test_event.html`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/javascripts/test_event.js` & `plone_app_event-5.1.3/plone/app/event/tests/javascripts/test_event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.css` & `plone_app_event-5.1.3/plone/app/event/tests/qunit/qunit.css`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/qunit/qunit.js` & `plone_app_event-5.1.3/plone/app/event/tests/qunit/qunit.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/robot/test_event_roundtrip.robot` & `plone_app_event-5.1.3/plone/app/event/tests/robot/test_event_roundtrip.robot`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/robot/variables.py` & `plone_app_event-5.1.3/plone/app/event/tests/robot/variables.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_base_module.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_base_module.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_catalog.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_dx_behaviors.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_dx_behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_event_listing.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_event_summary.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_event_view.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_ical_import.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_ical_import.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_icalendar.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_icalendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_portlet_calendar.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_portlet_events.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_portlet_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_recurrence.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/tests/test_search.py` & `plone_app_event-5.1.3/plone/app/event/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/upgrades/configure.zcml` & `plone_app_event-5.1.3/plone/app/event/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/upgrades/upgrades.py` & `plone_app_event-5.1.3/plone/app/event/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone/app/event/vocabularies.py` & `plone_app_event-5.1.3/plone/app/event/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone.app.event.egg-info/PKG-INFO` & `plone_app_event-5.1.3/plone.app.event.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.1.2
+Version: 5.1.3
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -155,14 +155,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.3 (2024-05-30)
+------------------
+
+Bug fixes:
+
+
+- Conditionally load the zcml for our portlets.
+  [maurits] (#3923)
+
+
 5.1.2 (2024-04-16)
 ------------------
 
 Bug fixes:
 
 
 - Fix calculation of eventaccessor urls @1letter (#387)
```

### Comparing `plone.app.event-5.1.2/plone.app.event.egg-info/SOURCES.txt` & `plone_app_event-5.1.3/plone.app.event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/plone.app.event.egg-info/requires.txt` & `plone_app_event-5.1.3/plone.app.event.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/pyproject.toml` & `plone_app_event-5.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.1.2/setup.py` & `plone_app_event-5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.1.2"
+version = "5.1.3"
 
 
 long_description = "\n\n".join(
     [
         Path("README.rst").read_text(),
         (Path(".") / "docs" / "installation.rst").read_text(),
         Path("CHANGES.rst").read_text(),
```

