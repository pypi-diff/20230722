# Comparing `tmp/embykeeper-2.3.3.tar.gz` & `tmp/embykeeper-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.3.3.tar", last modified: Thu Jul 20 17:21:15 2023, max compression
+gzip compressed data, was "embykeeper-2.3.4.tar", last modified: Sat Jul 22 14:44:29 2023, max compression
```

## Comparing `embykeeper-2.3.3.tar` & `embykeeper-2.3.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.145521 embykeeper-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 17:21:05.000000 embykeeper-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 17:21:05.000000 embykeeper-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24347 2023-07-20 17:21:15.141521 embykeeper-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23448 2023-07-20 17:21:05.000000 embykeeper-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.137521 embykeeper-2.3.3/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.137521 embykeeper-2.3.3/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.137521 embykeeper-2.3.3/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/bots/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24347 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:21:14.000000 embykeeper-2.3.3/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 17:21:15.000000 embykeeper-2.3.3/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.133521 embykeeper-2.3.3/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-20 17:21:05.000000 embykeeper-2.3.3/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-20 17:21:05.000000 embykeeper-2.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:21:15.145521 embykeeper-2.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:21:15.141521 embykeeper-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 17:21:05.000000 embykeeper-2.3.3/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-22 14:44:18.000000 embykeeper-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-22 14:44:18.000000 embykeeper-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24347 2023-07-22 14:44:29.403389 embykeeper-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23448 2023-07-22 14:44:18.000000 embykeeper-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.395389 embykeeper-2.3.4/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.399389 embykeeper-2.3.4/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.399389 embykeeper-2.3.4/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.399389 embykeeper-2.3.4/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17913 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/bots/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15276 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.399389 embykeeper-2.3.4/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.399389 embykeeper-2.3.4/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24347 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-22 14:44:29.000000 embykeeper-2.3.4/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.395389 embykeeper-2.3.4/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.395389 embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.395389 embykeeper-2.3.4/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-22 14:44:18.000000 embykeeper-2.3.4/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-22 14:44:18.000000 embykeeper-2.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 14:44:29.403389 embykeeper-2.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:44:29.403389 embykeeper-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-22 14:44:18.000000 embykeeper-2.3.4/tests/test_cli.py
```

### Comparing `embykeeper-2.3.3/LICENSE` & `embykeeper-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/PKG-INFO` & `embykeeper-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.3.3
+Version: 2.3.4
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.3.3 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.3.4 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
```

### Comparing `embykeeper-2.3.3/README.md` & `embykeeper-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/cli.py` & `embykeeper-2.3.4/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/data.py` & `embykeeper-2.3.4/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/embywatcher/emby.py` & `embykeeper-2.3.4/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/embywatcher/main.py` & `embykeeper-2.3.4/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/log.py` & `embykeeper-2.3.4/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/settings.py` & `embykeeper-2.3.4/embykeeper/settings.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/base.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/ljyy.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/ljyy.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/misty.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.3.4/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/link.py` & `embykeeper-2.3.4/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/log.py` & `embykeeper-2.3.4/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/main.py` & `embykeeper-2.3.4/embykeeper/telechecker/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,18 +59,23 @@
 
 def get_cls(type: str, names: List[str] = None) -> List[Type]:
     sub, suffix = get_spec(type)
     if names == None:
         names = get_names(type)
     results = []
     for name in names:
-        module = import_module(f"{__name__}.{sub}.{name}")
-        for cn, cls in inspect.getmembers(module, inspect.isclass):
-            if (name.replace("_", "") + suffix).lower() == cn.lower():
-                results.append(cls)
+        try:
+            module = import_module(f"{__name__}.{sub}.{name.lower()}")
+            for cn, cls in inspect.getmembers(module, inspect.isclass):
+                if (name.lower().replace("_", "") + suffix).lower() == cn.lower():
+                    results.append(cls)
+        except ImportError:
+            all_names = get_names(type)
+            logger.warning(f'您配置的 "{type}" 不支持站点 "{name}", 请从以下站点中选择:')
+            logger.warning(", ".join(all_names))
     return results
 
 
 def extract(clss: List[Type]) -> List[Type]:
     extracted = []
     for cls in clss:
         ncs = [c for c in cls.__dict__.values() if inspect.isclass(c)]
```

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/messager/base.py` & `embykeeper-2.3.4/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/messager/common.py` & `embykeeper-2.3.4/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.3.4/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/telechecker/tele.py` & `embykeeper-2.3.4/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper/utils.py` & `embykeeper-2.3.4/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.3.4/embykeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.3.3
+Version: 2.3.4
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.3.3 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.3.4 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: End Users/Desktop Classifier: Natural Language :: Chinese
 (Simplified) Classifier: License :: OSI Approved :: GNU General Public License
```

### Comparing `embykeeper-2.3.3/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.3.4/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/app.py` & `embykeeper-2.3.4/embykeeperweb/app.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/404.html` & `embykeeper-2.3.4/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.3.4/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.3.4/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.3.4/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.3.4/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.3.4/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.3.4/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/console.html` & `embykeeper-2.3.4/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/embykeeperweb/templates/login.html` & `embykeeper-2.3.4/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.3.3/pyproject.toml` & `embykeeper-2.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.3.3"
+version = "2.3.4"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-2.3.3/tests/test_cli.py` & `embykeeper-2.3.4/tests/test_cli.py`

 * *Files identical despite different names*

