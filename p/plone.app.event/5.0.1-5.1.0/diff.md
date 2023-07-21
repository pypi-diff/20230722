# Comparing `tmp/plone.app.event-5.0.1.tar.gz` & `tmp/plone.app.event-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.event-5.0.1.tar", last modified: Sat Apr 15 10:18:36 2023, max compression
+gzip compressed data, was "plone.app.event-5.1.0.tar", last modified: Fri Jul 21 23:18:04 2023, max compression
```

## Comparing `plone.app.event-5.0.1.tar` & `plone.app.event-5.1.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/
--rw-r--r--   0 gil       (1000) gil       (1000)    57519 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    18099 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      756 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/LICENSE.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      202 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)    61804 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)      587 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.475229 plone.app.event-5.0.1/docs/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.476229 plone.app.event-5.0.1/docs/api/
--rw-r--r--   0 gil       (1000) gil       (1000)       94 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/base.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.476229 plone.app.event-5.0.1/docs/api/browser/
--rw-r--r--   0 gil       (1000) gil       (1000)      145 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/event_listing.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      146 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/event_summary.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      136 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/event_view.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      148 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/formatted_date.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      158 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/browser/leadimage_viewlet.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.477229 plone.app.event-5.0.1/docs/api/dx/
--rw-r--r--   0 gil       (1000) gil       (1000)      118 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/dx/behaviors.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      121 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/dx/interfaces.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      119 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/dx/traverser.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.477229 plone.app.event-5.0.1/docs/api/ical/
--rw-r--r--   0 gil       (1000) gil       (1000)      122 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/ical/exporter.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      121 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/ical/importer.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      403 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/index.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      112 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/interfaces.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      113 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/api/recurrence.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     5633 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/architectural-overview.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      395 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/conf.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3464 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/designchoices.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    10346 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/development.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1590 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/index.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2839 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/installation.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      884 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/docs/tests.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.477229 plone.app.event-5.0.1/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.478229 plone.app.event-5.0.1/plone/app/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.479229 plone.app.event-5.0.1/plone/app/event/
--rw-r--r--   0 gil       (1000) gil       (1000)      369 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)    33259 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/base.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.480229 plone.app.event-5.0.1/plone/app/event/browser/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3398 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     5435 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_listing.pt
--rw-r--r--   0 gil       (1000) gil       (1000)    15434 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_listing.py
--rw-r--r--   0 gil       (1000) gil       (1000)     9639 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_summary.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     2965 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_summary.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1931 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_view.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      605 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/event_view.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3228 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/formatted_date.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1001 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/formatted_date.py
--rw-r--r--   0 gil       (1000) gil       (1000)      726 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/formatted_start_date.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      550 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/leadimage_viewlet.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.480229 plone.app.event-5.0.1/plone/app/event/browser/resources/
--rw-r--r--   0 gil       (1000) gil       (1000)      349 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/resources/calendar.svg
--rw-r--r--   0 gil       (1000) gil       (1000)     3726 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/browser/resources/event.js
--rw-r--r--   0 gil       (1000) gil       (1000)     2121 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/configure.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.481229 plone.app.event-5.0.1/plone/app/event/dx/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)    14257 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/behaviors.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1981 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      585 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/ical.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)      274 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      759 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/dx/traverser.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.481229 plone.app.event-5.0.1/plone/app/event/ical/
--rw-r--r--   0 gil       (1000) gil       (1000)      430 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3135 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)    14653 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/exporter.py
--rw-r--r--   0 gil       (1000) gil       (1000)    14459 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/ical/importer.py
--rw-r--r--   0 gil       (1000) gil       (1000)      350 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)      171 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/permissions.zcml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.482229 plone.app.event-5.0.1/plone/app/event/portlets/
--rw-r--r--   0 gil       (1000) gil       (1000)      767 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      836 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     4035 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.pt
--rw-r--r--   0 gil       (1000) gil       (1000)    11194 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3357 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     8198 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.473229 plone.app.event-5.0.1/plone/app/event/profiles/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/default/
--rw-r--r--   0 gil       (1000) gil       (1000)     2651 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/actions.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      157 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/browserlayer.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      357 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/controlpanel.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      321 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/metadata.xml
--rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/plone.app.event-default.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1194 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/portlets.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      479 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/registry.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      328 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/rolemap.xml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/default/types/
--rw-r--r--   0 gil       (1000) gil       (1000)      190 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types/Collection.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      186 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types/Folder.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      190 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types/Plone_Site.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      355 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/default/types.xml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/testing/
--rw-r--r--   0 gil       (1000) gil       (1000)      181 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/testing/metadata.xml
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.483229 plone.app.event-5.0.1/plone/app/event/profiles/testing/types/
--rw-r--r--   0 gil       (1000) gil       (1000)     2850 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
--rw-r--r--   0 gil       (1000) gil       (1000)      199 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/profiles/testing/types.xml
--rw-r--r--   0 gil       (1000) gil       (1000)     6714 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/recurrence.py
--rw-r--r--   0 gil       (1000) gil       (1000)      567 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/recurrence.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     2462 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/setuphandlers.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3694 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/testing.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.485229 plone.app.event-5.0.1/plone/app/event/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)      898 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/INACTIVE_test_robot.py
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5753 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/base_setup.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2201 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/icaltest.ics
--rw-r--r--   0 gil       (1000) gil       (1000)     2202 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/icaltest2.ics
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.485229 plone.app.event-5.0.1/plone/app/event/tests/javascripts/
--rw-r--r--   0 gil       (1000) gil       (1000)    23860 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.html
--rw-r--r--   0 gil       (1000) gil       (1000)      715 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.js
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.485229 plone.app.event-5.0.1/plone/app/event/tests/qunit/
--rw-r--r--   0 gil       (1000) gil       (1000)     3952 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.css
--rw-r--r--   0 gil       (1000) gil       (1000)    37060 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.js
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/plone/app/event/tests/robot/
--rw-r--r--   0 gil       (1000) gil       (1000)     6114 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/robot/test_event_roundtrip.robot
--rw-r--r--   0 gil       (1000) gil       (1000)      633 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/robot/variables.py
--rw-r--r--   0 gil       (1000) gil       (1000)    35328 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/test_base_module.py
--rw-r--r--   0 gil       (1000) gil       (1000)      773 2023-04-15 10:18:35.000000 plone.app.event-5.0.1/plone/app/event/tests/test_catalog.py
--rw-r--r--   0 gil       (1000) gil       (1000)    22380 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_dx_behaviors.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6395 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_event_listing.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4982 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_event_summary.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2075 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_event_view.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3583 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_ical_import.py
--rw-r--r--   0 gil       (1000) gil       (1000)    19302 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_icalendar.py
--rw-r--r--   0 gil       (1000) gil       (1000)     9253 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_portlet_calendar.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8861 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_portlet_events.py
--rw-r--r--   0 gil       (1000) gil       (1000)    13916 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_recurrence.py
--rw-r--r--   0 gil       (1000) gil       (1000)      544 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/tests/test_search.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/plone/app/event/upgrades/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/upgrades/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)      969 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/upgrades/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     3415 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/upgrades/upgrades.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1261 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone/app/event/vocabularies.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 10:18:36.478229 plone.app.event-5.0.1/plone.app.event.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)    61804 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     4246 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      711 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/plone.app.event.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     2934 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      276 2023-04-15 10:18:36.486230 plone.app.event-5.0.1/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     2527 2023-04-15 10:18:36.000000 plone.app.event-5.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.066173 plone.app.event-5.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    57719 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18099 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      756 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    62041 2023-07-21 23:18:04.065895 plone.app.event-5.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      587 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.032905 plone.app.event-5.1.0/docs/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.034437 plone.app.event-5.1.0/docs/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/base.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.036097 plone.app.event-5.1.0/docs/api/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/browser/event_listing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/browser/event_summary.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      136 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/browser/event_view.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/browser/formatted_date.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      158 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/browser/leadimage_viewlet.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.037007 plone.app.event-5.1.0/docs/api/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)      118 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/dx/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/dx/interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      119 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/dx/traverser.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.037596 plone.app.event-5.1.0/docs/api/ical/
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/ical/exporter.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      121 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/ical/importer.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      112 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      113 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/api/recurrence.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5633 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/architectural-overview.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3464 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/designchoices.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10346 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/development.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1590 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2839 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/installation.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      884 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/docs/tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.037847 plone.app.event-5.1.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.040488 plone.app.event-5.1.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.043825 plone.app.event-5.1.0/plone/app/event/
+-rw-r--r--   0 maurits    (501) staff       (20)      369 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    33259 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/base.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.047326 plone.app.event-5.1.0/plone/app/event/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5435 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/event_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    15434 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/event_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9719 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/event_summary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2965 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/event_summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/event_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      605 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/event_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3228 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/formatted_date.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1001 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/formatted_date.py
+-rw-r--r--   0 maurits    (501) staff       (20)      726 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/formatted_start_date.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/leadimage_viewlet.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.047913 plone.app.event-5.1.0/plone/app/event/browser/resources/
+-rw-r--r--   0 maurits    (501) staff       (20)      349 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/resources/calendar.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     3726 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/browser/resources/event.js
+-rw-r--r--   0 maurits    (501) staff       (20)     2121 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.050041 plone.app.event-5.1.0/plone/app/event/dx/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/dx/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14257 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/dx/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1981 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/dx/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      585 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/dx/ical.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/dx/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/dx/traverser.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.051487 plone.app.event-5.1.0/plone/app/event/ical/
+-rw-r--r--   0 maurits    (501) staff       (20)      430 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/ical/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3135 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/ical/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    14653 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/ical/exporter.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14459 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/ical/importer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      350 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      171 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.053135 plone.app.event-5.1.0/plone/app/event/portlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      767 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/portlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      836 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/portlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4035 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/portlets/portlet_calendar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    11194 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/portlets/portlet_calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3357 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/portlets/portlet_events.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9912 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/portlets/portlet_events.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.026970 plone.app.event-5.1.0/plone/app/event/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.055587 plone.app.event-5.1.0/plone/app/event/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     2651 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      157 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      357 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      321 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/plone.app.event-default.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1194 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      479 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      328 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.056422 plone.app.event-5.1.0/plone/app/event/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/types/Collection.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/types/Plone_Site.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      355 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.057006 plone.app.event-5.1.0/plone/app/event/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      181 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.057262 plone.app.event-5.1.0/plone/app/event/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2850 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     6714 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      567 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/recurrence.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2462 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3694 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.062987 plone.app.event-5.1.0/plone/app/event/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)      898 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/INACTIVE_test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5753 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/base_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/icaltest.ics
+-rw-r--r--   0 maurits    (501) staff       (20)     2202 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/icaltest2.ics
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.063582 plone.app.event-5.1.0/plone/app/event/tests/javascripts/
+-rw-r--r--   0 maurits    (501) staff       (20)    23860 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/javascripts/test_event.html
+-rw-r--r--   0 maurits    (501) staff       (20)      715 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/javascripts/test_event.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.064204 plone.app.event-5.1.0/plone/app/event/tests/qunit/
+-rw-r--r--   0 maurits    (501) staff       (20)     3952 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/qunit/qunit.css
+-rw-r--r--   0 maurits    (501) staff       (20)    37060 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/qunit/qunit.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.064757 plone.app.event-5.1.0/plone/app/event/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     6114 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/robot/test_event_roundtrip.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      633 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/robot/variables.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35328 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_base_module.py
+-rw-r--r--   0 maurits    (501) staff       (20)      773 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22380 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_dx_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6395 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_event_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4982 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_event_summary.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2075 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_event_view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3583 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_ical_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19302 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_icalendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9253 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_portlet_calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8861 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_portlet_events.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13916 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_recurrence.py
+-rw-r--r--   0 maurits    (501) staff       (20)      544 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/tests/test_search.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.065488 plone.app.event-5.1.0/plone/app/event/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      969 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3415 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/upgrades/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1261 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone/app/event/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-21 23:18:04.040238 plone.app.event-5.1.0/plone.app.event.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    62041 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4236 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      705 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/plone.app.event.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3873 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-21 23:18:04.066240 plone.app.event-5.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2593 2023-07-21 23:18:03.000000 plone.app.event-5.1.0/setup.py
```

### Comparing `plone.app.event-5.0.1/CHANGES.rst` & `plone.app.event-5.1.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.0 (2023-07-22)
+------------------
+
+New features:
+
+
+- Cache the events from the 'Upcoming Events' portlet
+  [frapell] (#351)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5ed054fb)
+
+
 5.0.1 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files and dependencies.
```

### Comparing `plone.app.event-5.0.1/LICENSE.GPL` & `plone.app.event-5.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/LICENSE.rst` & `plone.app.event-5.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/PKG-INFO` & `plone.app.event-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.0.1
+Version: 5.1.0
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 plone.app.event
 ===============
 
@@ -115,14 +116,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.0 (2023-07-22)
+------------------
+
+New features:
+
+
+- Cache the events from the 'Upcoming Events' portlet
+  [frapell] (#351)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5ed054fb)
+
+
 5.0.1 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files and dependencies.
```

### Comparing `plone.app.event-5.0.1/README.rst` & `plone.app.event-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/docs/architectural-overview.rst` & `plone.app.event-5.1.0/docs/architectural-overview.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/docs/designchoices.rst` & `plone.app.event-5.1.0/docs/designchoices.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/docs/development.rst` & `plone.app.event-5.1.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/docs/index.rst` & `plone.app.event-5.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/docs/installation.rst` & `plone.app.event-5.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/docs/tests.rst` & `plone.app.event-5.1.0/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/base.py` & `plone.app.event-5.1.0/plone/app/event/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/configure.zcml` & `plone.app.event-5.1.0/plone/app/event/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/event_listing.pt` & `plone.app.event-5.1.0/plone/app/event/browser/event_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/event_listing.py` & `plone.app.event-5.1.0/plone/app/event/browser/event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/event_summary.pt` & `plone.app.event-5.1.0/plone/app/event/browser/event_summary.pt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
               >When</strong>
               <p class="card-text h5">
                 <span>
                   <tal:date replace="structure python:view.formatted_date(context)" />
                 </span>
                 <span class="timezone text-muted small"
                       tal:condition="start_tzname"
+                      i18n:ignore="True"
                 >
                   (<tal:tzname replace="start_tzname">timezone name</tal:tzname>
                   / UTC<tal:tzoffset replace="start_utcoffset" />)
                 </span>
               </p>
             </div>
           </div>
@@ -235,14 +236,15 @@
                   <a href="#"
                      rel="nofollow"
                      title="Download this event in iCal format"
                      tal:attributes="
                        href string:$here_url/ics_view;
                      "
                      i18n:attributes="title title_add_to_ical;"
+                     i18n:translate=""
                   >iCal</a>
                 </p>
               </div>
             </div>
           </div>
 
         </div>
```

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/event_summary.py` & `plone.app.event-5.1.0/plone/app/event/browser/event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/event_view.pt` & `plone.app.event-5.1.0/plone/app/event/browser/event_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/event_view.py` & `plone.app.event-5.1.0/plone/app/event/browser/event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/formatted_date.pt` & `plone.app.event-5.1.0/plone/app/event/browser/formatted_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/formatted_date.py` & `plone.app.event-5.1.0/plone/app/event/browser/formatted_date.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/formatted_start_date.pt` & `plone.app.event-5.1.0/plone/app/event/browser/formatted_start_date.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/leadimage_viewlet.py` & `plone.app.event-5.1.0/plone/app/event/browser/leadimage_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/browser/resources/event.js` & `plone.app.event-5.1.0/plone/app/event/browser/resources/event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/configure.zcml` & `plone.app.event-5.1.0/plone/app/event/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/dx/behaviors.py` & `plone.app.event-5.1.0/plone/app/event/dx/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/dx/configure.zcml` & `plone.app.event-5.1.0/plone/app/event/dx/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/dx/ical.zcml` & `plone.app.event-5.1.0/plone/app/event/dx/ical.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/dx/traverser.py` & `plone.app.event-5.1.0/plone/app/event/dx/traverser.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/ical/configure.zcml` & `plone.app.event-5.1.0/plone/app/event/ical/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/ical/exporter.py` & `plone.app.event-5.1.0/plone/app/event/ical/exporter.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/ical/importer.py` & `plone.app.event-5.1.0/plone/app/event/ical/importer.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/portlets/__init__.py` & `plone.app.event-5.1.0/plone/app/event/portlets/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/portlets/configure.zcml` & `plone.app.event-5.1.0/plone/app/event/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.pt` & `plone.app.event-5.1.0/plone/app/event/portlets/portlet_calendar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/portlets/portlet_calendar.py` & `plone.app.event-5.1.0/plone/app/event/portlets/portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.pt` & `plone.app.event-5.1.0/plone/app/event/portlets/portlet_events.pt`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/portlets/portlet_events.py` & `plone.app.event-5.1.0/plone/app/event/portlets/portlet_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,76 @@
 from plone.app.event.portlets import get_calendar_url
 from plone.app.event.portlets.portlet_calendar import ISyndicatableCollection
 from plone.app.event.portlets.portlet_calendar import search_base_uid_source
 from plone.app.portlets.portlets import base
 from plone.app.querystring import queryparser
 from plone.app.uuid.utils import uuidToObject
 from plone.base.interfaces.controlpanel import ISiteSchema
+from plone.event.interfaces import IEvent
+from plone.memoize import ram
 from plone.memoize.compress import xhtml_compress
 from plone.portlets.interfaces import IPortletDataProvider
 from plone.registry.interfaces import IRegistry
+from Products.CMFCore.utils import getToolByName
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zExceptions import NotFound
 from zope import schema
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.component.hooks import getSite
 from zope.contentprovider.interfaces import IContentProvider
 from zope.interface import implementer
 
 
+def _render_events_cachekey(method, self):
+    # Since the events portlet shows the upcoming events, we simply get the
+    # most recently modified event and return its uuid and last modified date
+    # as key. If there is a change, then the most expensive computation can be
+    # performed.
+
+    site = getSite()
+    cat = getToolByName(site, "portal_catalog")
+
+    query = {}
+    data = self.data
+    if data.state:
+        query["review_state"] = data.state
+
+    start = localized_now(site)
+
+    query.update(self.request.get("contentFilter", {}))
+    if ISyndicatableCollection and ISyndicatableCollection.providedBy(self.search_base):
+        # Whatever sorting is defined, we're overriding it.
+        query = queryparser.parseFormquery(
+            self.search_base, self.search_base.query, sort_on="start", sort_order=None
+        )
+        if "start" in query:
+            start = query["start"]
+    elif self.search_base_path:
+        query["path"] = {"query": self.search_base_path}
+
+    # Any object with an IEvent interface.
+    query["object_provides"] = IEvent.__identifier__
+    # Only upcoming events.
+    query.update(start_end_query(start=start, end=None))
+    # We want to get the next data.count events, just as the portlet would.
+    query["sort_on"] = "start"
+    query["sort_order"] = "asc"
+    query["sort_limit"] = data.count
+
+    events = cat(**query)
+    uuid = ""
+    modified = 0
+    for event in events:
+        uuid += event.UID
+        modified += event.modified.asdatetime().timestamp()
+
+    return (uuid, modified)
+
+
 class IEventsPortlet(IPortletDataProvider):
     count = schema.Int(
         title=_("Number of items to display"),
         description=_("How many items to list."),
         required=True,
         default=5,
         min=1,
@@ -141,14 +190,15 @@
         return xhtml_compress(self._template())
 
     @property
     def available(self):
         return self.data.count > 0 and len(self.events)
 
     @property
+    @ram.cache(_render_events_cachekey)
     def events(self):
         context = aq_inner(self.context)
         data = self.data
 
         query = {}
         if data.state:
             query["review_state"] = data.state
```

### Comparing `plone.app.event-5.0.1/plone/app/event/profiles/default/actions.xml` & `plone.app.event-5.1.0/plone/app/event/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/profiles/default/portlets.xml` & `plone.app.event-5.1.0/plone/app/event/profiles/default/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml` & `plone.app.event-5.1.0/plone/app/event/profiles/testing/types/plone.app.event.dx.event.xml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/recurrence.py` & `plone.app.event-5.1.0/plone/app/event/recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/recurrence.zcml` & `plone.app.event-5.1.0/plone/app/event/recurrence.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/setuphandlers.py` & `plone.app.event-5.1.0/plone/app/event/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/testing.py` & `plone.app.event-5.1.0/plone/app/event/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/INACTIVE_test_robot.py` & `plone.app.event-5.1.0/plone/app/event/tests/INACTIVE_test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/base_setup.py` & `plone.app.event-5.1.0/plone/app/event/tests/base_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/icaltest.ics` & `plone.app.event-5.1.0/plone/app/event/tests/icaltest.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/icaltest2.ics` & `plone.app.event-5.1.0/plone/app/event/tests/icaltest2.ics`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.html` & `plone.app.event-5.1.0/plone/app/event/tests/javascripts/test_event.html`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/javascripts/test_event.js` & `plone.app.event-5.1.0/plone/app/event/tests/javascripts/test_event.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.css` & `plone.app.event-5.1.0/plone/app/event/tests/qunit/qunit.css`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/qunit/qunit.js` & `plone.app.event-5.1.0/plone/app/event/tests/qunit/qunit.js`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/robot/test_event_roundtrip.robot` & `plone.app.event-5.1.0/plone/app/event/tests/robot/test_event_roundtrip.robot`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/robot/variables.py` & `plone.app.event-5.1.0/plone/app/event/tests/robot/variables.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_base_module.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_base_module.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_catalog.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_dx_behaviors.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_dx_behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_event_listing.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_event_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_event_summary.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_event_summary.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_event_view.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_event_view.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_ical_import.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_ical_import.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_icalendar.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_icalendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_portlet_calendar.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_portlet_calendar.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_portlet_events.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_portlet_events.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_recurrence.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/tests/test_search.py` & `plone.app.event-5.1.0/plone/app/event/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/upgrades/configure.zcml` & `plone.app.event-5.1.0/plone/app/event/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/upgrades/upgrades.py` & `plone.app.event-5.1.0/plone/app/event/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone/app/event/vocabularies.py` & `plone.app.event-5.1.0/plone/app/event/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.event-5.0.1/plone.app.event.egg-info/PKG-INFO` & `plone.app.event-5.1.0/plone.app.event.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.event
-Version: 5.0.1
+Version: 5.1.0
 Summary: The Plone calendar framework
 Home-page: https://github.com/plone/plone.app.event
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone event
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,16 @@
 Classifier: Framework :: Plone :: Core
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 plone.app.event
 ===============
 
@@ -115,14 +116,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.1.0 (2023-07-22)
+------------------
+
+New features:
+
+
+- Cache the events from the 'Upcoming Events' portlet
+  [frapell] (#351)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (5ed054fb)
+
+
 5.0.1 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files and dependencies.
```

### Comparing `plone.app.event-5.0.1/plone.app.event.egg-info/SOURCES.txt` & `plone.app.event-5.1.0/plone.app.event.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 CHANGES.rst
 CONTRIBUTING.rst
 LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/architectural-overview.rst
 docs/conf.py
 docs/designchoices.rst
 docs/development.rst
 docs/index.rst
 docs/installation.rst
```

### Comparing `plone.app.event-5.0.1/plone.app.event.egg-info/requires.txt` & `plone.app.event-5.1.0/plone.app.event.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 setuptools
 plone.base
 Products.statusmessages
 icalendar
 Products.DateRecurringIndex
 Products.ZCatalog
+Products.GenericSetup
 plone.app.contenttypes
 plone.app.uuid
 plone.resource
 plone.app.contentlisting
 plone.app.dexterity
 plone.app.portlets>=2.5.1
 plone.app.querystring
@@ -24,17 +25,16 @@
 plone.formwidget.recurrence[z3cform]>=1.2.4
 plone.indexer
 plone.memoize
 plone.namedfile
 plone.portlets
 plone.supermodel
 plone.uuid
-plone.z3cform
 pytz
 z3c.form>=3.2.1
-zope.globalrequest
+Zope
 
 [test]
 plone.app.robotframework
 plone.app.testing[robot]
 plone.testing
 robotsuite
```

### Comparing `plone.app.event-5.0.1/setup.py` & `plone.app.event-5.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
-import os
 
-
-version = "5.0.1"
+version = "5.1.0"
 
 
 long_description = "\n\n".join(
     [
-        open("README.rst").read(),
-        open(os.path.join("docs", "installation.rst")).read(),
-        open("CHANGES.rst").read(),
+        Path("README.rst").read_text(),
+        (Path(".") / "docs" / "installation.rst").read_text(),
+        Path("CHANGES.rst").read_text(),
     ]
 )
 
 
 setup(
     name="plone.app.event",
     version=version,
     description="The Plone calendar framework",
     long_description=long_description,
+    long_description_content_type="text/x-rst",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Programming Language :: Python",
@@ -37,23 +37,24 @@
     author="Plone Foundation",
     author_email="plone-developers@lists.sourceforge.net",
     url="https://github.com/plone/plone.app.event",
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     install_requires=[
         "setuptools",
         "plone.base",
         "Products.statusmessages",
         "icalendar",  # >4.0.2
         "Products.DateRecurringIndex",
         "Products.ZCatalog",
+        "Products.GenericSetup",
         "plone.app.contenttypes",
         "plone.app.uuid",
         "plone.resource",
         "plone.app.contentlisting",
         "plone.app.dexterity",
         "plone.app.portlets >= 2.5.1",
         "plone.app.querystring",
@@ -70,18 +71,17 @@
         "plone.formwidget.recurrence [z3cform] >= 1.2.4",
         "plone.indexer",
         "plone.memoize",
         "plone.namedfile",
         "plone.portlets",
         "plone.supermodel",
         "plone.uuid",
-        "plone.z3cform",
         "pytz",
         "z3c.form >= 3.2.1",
-        "zope.globalrequest",
+        "Zope",
     ],
     extras_require={
         "test": [
             "plone.app.robotframework",
             "plone.app.testing [robot]",
             "plone.testing",
             "robotsuite",
```

