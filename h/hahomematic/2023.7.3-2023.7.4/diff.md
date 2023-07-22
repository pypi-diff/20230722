# Comparing `tmp/hahomematic-2023.7.3.tar.gz` & `tmp/hahomematic-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.3.tar", last modified: Fri Jul 14 09:34:32 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.4.tar", last modified: Sat Jul 22 21:30:00 2023, max compression
```

## Comparing `hahomematic-2023.7.3.tar` & `hahomematic-2023.7.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24363 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    53614 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:34:32.285365 hahomematic-2023.7.3/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-14 09:34:31.000000 hahomematic-2023.7.3/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-14 09:34:32.000000 hahomematic-2023.7.3/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:34:31.000000 hahomematic-2023.7.3/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:34:30.000000 hahomematic-2023.7.3/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 09:34:32.000000 hahomematic-2023.7.3/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 09:34:32.000000 hahomematic-2023.7.3/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-14 09:33:58.000000 hahomematic-2023.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-14 09:34:32.289365 hahomematic-2023.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.582215 hahomematic-2023.7.4/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54098 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26742 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 21:30:00.586215 hahomematic-2023.7.4/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-22 21:29:59.000000 hahomematic-2023.7.4/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 21:29:58.000000 hahomematic-2023.7.4/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 21:30:00.000000 hahomematic-2023.7.4/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-22 21:29:27.000000 hahomematic-2023.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-22 21:30:00.590215 hahomematic-2023.7.4/setup.cfg
```

### Comparing `hahomematic-2023.7.3/LICENSE` & `hahomematic-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/PKG-INFO` & `hahomematic-2023.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.3/README.md` & `hahomematic-2023.7.4/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/__init__.py` & `hahomematic-2023.7.4/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/backport.py` & `hahomematic-2023.7.4/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.4/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/caches/persistent.py` & `hahomematic-2023.7.4/hahomematic/caches/persistent.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
             channel_name = str(
                 self.get_device_parameter(
                     interface_id=interface_id,
                     device_address=channel_address,
                     parameter=HM_TYPE,
                 )
             )
-            channels[channel_address] = Channel(type=channel_name)
+            channels[channel_address] = Channel(type=channel_name, address=channel_address)
 
         return channels
 
     def get_device_descriptions(self, interface_id: str) -> dict[str, dict[str, Any]]:
         """Return the devices by interface."""
         return self._device_descriptions.get(interface_id, {})
```

### Comparing `hahomematic-2023.7.3/hahomematic/caches/visibility.py` & `hahomematic-2023.7.4/hahomematic/caches/visibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from functools import lru_cache
 import logging
 import os
 from typing import Any, Final
 
 from hahomematic import central_unit as hmcu, support as hms
 from hahomematic.const import (
+    CLICK_EVENTS,
     DEFAULT_ENCODING,
     EVENT_CONFIG_PENDING,
     EVENT_ERROR,
     EVENT_STICKY_UN_REACH,
     EVENT_UN_REACH,
     EVENT_UPDATE_PENDING,
     FILE_CUSTOM_UN_IGNORE_PARAMETERS,
@@ -64,14 +65,21 @@
     "HmIPW-WTH": ((1,), (PARAM_TEMPERATURE_MAXIMUM, PARAM_TEMPERATURE_MINIMUM)),
 }
 
 # Some parameters are marked as INTERNAL in the paramset and not considered by default,
 # but some are required and should be added here.
 ALLOWED_INTERNAL_PARAMETERS: Final = ("DIRECTION",)
 
+
+# Ignore events for some devices
+_IGNORE_DEVICES_FOR_ENTITY_EVENTS: Final[dict[str, tuple[str, ...]]] = {
+    "HmIP-PS": CLICK_EVENTS,
+}
+
+
 # Entities that will be created, but should be hidden.
 _HIDDEN_PARAMETERS: Final[tuple[str, ...]] = (
     EVENT_CONFIG_PENDING,
     EVENT_ERROR,
     EVENT_STICKY_UN_REACH,
     EVENT_UN_REACH,
     EVENT_UPDATE_PENDING,
@@ -266,14 +274,19 @@
             PARAMSET_KEY_VALUES: set(),
         }
         self._ignore_parameters_by_device_lower: Final[dict[str, tuple[str, ...]]] = {
             parameter: tuple(device_type.lower() for device_type in device_types)
             for parameter, device_types in _IGNORE_PARAMETERS_BY_DEVICE.items()
         }
 
+        self._ignore_devices_for_entity_events_lower: Final[dict[str, tuple[str, ...]]] = {
+            device_type.lower(): tuple(event for event in events)
+            for device_type, events in _IGNORE_DEVICES_FOR_ENTITY_EVENTS.items()
+        }
+
         self._un_ignore_parameters_by_device_lower: Final[dict[str, tuple[str, ...]]] = {
             device_type.lower(): parameters
             for device_type, parameters in _UN_IGNORE_PARAMETERS_BY_DEVICE.items()
         }
 
         # device_type, channel_no, paramset_key, set[parameter]
         self._un_ignore_parameters_by_device_paramset_key: Final[
@@ -357,22 +370,31 @@
                 paramset_key=paramset_key,
                 parameter=parameter,
             ):
                 return False
 
             if (
                 (
-                    parameter in _IGNORED_PARAMETERS
-                    or parameter.endswith(tuple(_IGNORED_PARAMETERS_WILDCARDS_END))
-                    or parameter.startswith(tuple(_IGNORED_PARAMETERS_WILDCARDS_START))
+                    (
+                        parameter in _IGNORED_PARAMETERS
+                        or parameter.endswith(tuple(_IGNORED_PARAMETERS_WILDCARDS_END))
+                        or parameter.startswith(tuple(_IGNORED_PARAMETERS_WILDCARDS_START))
+                    )
+                    and parameter not in self._required_parameters
+                )
+                or hms.element_matches_key(
+                    search_elements=self._ignore_parameters_by_device_lower.get(parameter, []),
+                    compare_with=device_type_l,
+                )
+                or hms.element_matches_key(
+                    search_elements=self._ignore_devices_for_entity_events_lower,
+                    compare_with=parameter,
+                    search_key=device_type_l,
+                    do_wildcard_search=False,
                 )
-                and parameter not in self._required_parameters
-            ) or hms.element_matches_key(
-                search_elements=self._ignore_parameters_by_device_lower.get(parameter, []),
-                compare_with=device_type_l,
             ):
                 return True
 
             if (
                 accept_channel := _ACCEPT_PARAMETER_ONLY_ON_CHANNEL.get(parameter)
             ) is not None and accept_channel != channel_no:
                 return True
```

### Comparing `hahomematic-2023.7.3/hahomematic/central_unit.py` & `hahomematic-2023.7.4/hahomematic/central_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,21 +142,25 @@
         self._devices: Final[dict[str, HmDevice]] = {}
         # {sysvar_name, sysvar_entity}
         self.sysvar_entities: Final[dict[str, GenericSystemVariable]] = {}
         # {sysvar_name, program_button}U
         self.program_entities: Final[dict[str, HmProgramButton]] = {}
         # store last event received datetime by interface
         self.last_events: Final[dict[str, datetime]] = {}
-        # Signature: (name, *args) #CC
+        # Signature: (name, *args)
+        # e.g. DEVICES_CREATED, HUB_REFRESHED
         self._callback_system_event: Final[set[Callable]] = set()
-        # Signature: (interface_id, channel_address, parameter, value) #CC
+        # Signature: (interface_id, channel_address, parameter, value)
+        # Re-Fired events from CCU for parameter updates
         self._callback_entity_event: Final[set[Callable]] = set()
-        # Signature: (interface_id, entity) #CC
+        # Signature: (interface_id, entity)
+        # Fires parameter data updates as events with entity.
         self._callback_entity_data_event: Final[set[Callable]] = set()
-        # Signature: (event_type, event_data) #CC
+        # Signature: (event_type, event_data)
+        # Events like INTERFACE, KEYPRESS, ...
         self._callback_ha_event: Final[set[Callable]] = set()
 
         self.json_rpc_client: Final[JsonRpcAioHttpClient] = central_config.create_json_rpc_client()
 
         CENTRAL_INSTANCES[self._attr_name] = self
         self._connection_checker: Final = ConnectionChecker(self)
         self._hub: HmHub = HmHub(central=self)
@@ -522,23 +526,23 @@
         """Return all entities by platform. #CC."""
         if not existing_unique_ids:
             existing_unique_ids = []
         entities = []
         for entity in self._entities.values():
             if (
                 entity.unique_identifier not in existing_unique_ids
-                and entity.usage != HmEntityUsage.ENTITY_NO_CREATE
+                and entity.usage != HmEntityUsage.NO_CREATE
                 and entity.platform == platform
             ):
                 entities.append(entity)
 
         return entities
 
     def get_readable_entities(self) -> list[BaseEntity]:
-        """Return a list of readable entities. This also includes custom entities."""
+        """Return a list of readable entities."""
         readable_entities: list[BaseEntity] = []
         for entity in self._entities.values():
             if (isinstance(entity, GenericEntity) and entity.is_readable) or isinstance(
                 entity, CustomEntity
             ):
                 readable_entities.append(entity)
         return readable_entities
@@ -1029,15 +1033,19 @@
 
     def unregister_ha_event_callback(self, callback_handler: Callable) -> None:
         """RUn register ha_event callback in central."""
         if callback_handler in self._callback_ha_event:
             self._callback_ha_event.remove(callback_handler)
 
     def fire_ha_event_callback(self, event_type: HmEventType, event_data: dict[str, str]) -> None:
-        """Fire ha_event callback in central."""
+        """
+        Fire ha_event callback in central.
+
+        # Events like INTERFACE, KEYPRESS, ...
+        """
         for callback_handler in self._callback_ha_event:
             try:
                 callback_handler(event_type, event_data)
             except Exception as ex:
                 _LOGGER.error("FIRE_HA_EVENT_CALLBACK: Unable to call handler: %s", ex.args)
 
     def register_entity_event_callback(self, callback_handler: Callable) -> None:
@@ -1048,15 +1056,20 @@
         """Un register entity_event callback in central."""
         if callback_handler in self._callback_entity_event:
             self._callback_entity_event.remove(callback_handler)
 
     def fire_entity_event_callback(
         self, interface_id: str, channel_address: str, parameter: str, value: Any
     ) -> None:
-        """Fire entity callback in central."""
+        """
+        Fire entity callback in central.
+
+        Not used by HA.
+        Re-Fired events from CCU for parameter updates.
+        """
         for callback_handler in self._callback_entity_event:
             try:
                 callback_handler(interface_id, channel_address, parameter, value)
             except Exception as ex:
                 _LOGGER.error("FIRE_ENTITY_EVENT_CALLBACK: Unable to call handler: %s", ex.args)
 
     def register_entity_data_event_callback(self, callback_handler: Callable) -> None:
@@ -1065,15 +1078,20 @@
 
     def unregister_entity_data_event_callback(self, callback_handler: Callable) -> None:
         """Un register entity_event callback in central."""
         if callback_handler in self._callback_entity_data_event:
             self._callback_entity_data_event.remove(callback_handler)
 
     def fire_entity_data_event_callback(self, interface_id: str, entity: BaseEntity) -> None:
-        """Fire entity_data callback in central."""
+        """
+        Fire entity_data callback in central.
+
+        Not used by HA.
+        Fires parameter data updates as events with entity.
+        """
         for callback_handler in self._callback_entity_data_event:
             try:
                 callback_handler(interface_id, entity)
             except Exception as ex:
                 _LOGGER.error(
                     "FIRE_ENTITY_DATA_EVENT_CALLBACK: Unable to call handler: %s", ex.args
                 )
@@ -1084,15 +1102,19 @@
 
     def unregister_system_event_callback(self, callback_handler: Callable) -> None:
         """Un register system_event callback in central."""
         if callback_handler in self._callback_system_event:
             self._callback_system_event.remove(callback_handler)
 
     def fire_system_event_callback(self, name: str, **kwargs: Any) -> None:
-        """Fire system_event callback in central."""
+        """
+        Fire system_event callback in central.
+
+        e.g. DEVICES_CREATED, HUB_REFRESHED
+        """
         for callback_handler in self._callback_system_event:
             try:
                 callback_handler(name, **kwargs)
             except Exception as ex:
                 _LOGGER.error("FIRE_SYSTEM_EVENT_CALLBACK: Unable to call handler: %s", ex.args)
```

### Comparing `hahomematic-2023.7.3/hahomematic/client.py` & `hahomematic-2023.7.4/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/const.py` & `hahomematic-2023.7.4/hahomematic/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,26 @@
 DEFAULT_VERIFY_TLS: Final = False
 
 # Password can be empty.
 # Allowed characters: A-Z, a-z, 0-9, .!$():;#-
 # The CCU WebUI also supports ÄäÖöÜüß, but these characters are not supported by the XmlRPC servers
 CCU_PASSWORD_PATTERN: Final = r"[A-Za-z0-9.!$():;#-]{0,}"
 
+IDENTIFIER_SEPARATOR: Final = "@"
 INIT_DATETIME: Final = datetime.strptime("01.01.1970 00:00:00", "%d.%m.%Y %H:%M:%S")
 IP_ANY_V4: Final = "0.0.0.0"
 IP_ANY_V6: Final = "::"
 IP_LOCALHOST_V4: Final = "127.0.0.1"
 IP_LOCALHOST_V6: Final = "::1"
 PORT_ANY: Final = 0
 
+MANUFACTURER_EQ3: Final = "eQ-3"
+MANUFACTURER_HB: Final = "Homebrew"
+MANUFACTURER_MOEHLENHOFF: Final = "Möhlenhoff"
+
 PATH_JSON_RPC: Final = "/api/homematic.cgi"
 
 BACKEND_CCU: Final = "CCU"
 BACKEND_HOMEGEAR: Final = "Homegear"
 BACKEND_LOCAL: Final = "Local CCU"
 BACKEND_PYDEVCCU: Final = "PyDevCCU"
 LOCAL_INTERFACE = "Local"
@@ -223,15 +228,14 @@
 
 DEVICE_ERROR_EVENTS: Final[tuple[str, ...]] = ("ERROR", "SENSOR_ERROR")
 
 IMPULSE_EVENTS: Final[tuple[str, ...]] = (EVENT_SEQUENCE_OK,)
 
 BUTTON_ACTIONS: Final[tuple[str, ...]] = ("RESET_MOTION", "RESET_PRESENCE")
 
-
 FIX_UNIT_REPLACE: Final[dict[str, str]] = {
     '"': "",
     "100%": "%",
     "% rF": "%",
     "degree": "°C",
     "Lux": "lx",
     "m3": "m³",
@@ -343,16 +347,16 @@
 class HmEntityUsage(StrEnum):
     """Enum with information about usage in Home Assistant."""
 
     CE_PRIMARY: Final = "ce_primary"
     CE_SECONDARY: Final = "ce_secondary"
     CE_VISIBLE: Final = "ce_visible"
     ENTITY: Final = "entity"
-    ENTITY_NO_CREATE: Final = "entity_no_create"
     EVENT: Final = "event"
+    NO_CREATE: Final = "entity_no_create"
 
 
 class HmDeviceFirmwareState(StrEnum):
     """Enum with homematic device firmware states."""
 
     UP_TO_DATE: Final = "UP_TO_DATE"
     LIVE_UP_TO_DATE: Final = "LIVE_UP_TO_DATE"
@@ -448,14 +452,15 @@
 
 
 AVAILABLE_HM_PLATFORMS: Final[tuple[HmPlatform, ...]] = (
     HmPlatform.BINARY_SENSOR,
     HmPlatform.BUTTON,
     HmPlatform.CLIMATE,
     HmPlatform.COVER,
+    HmPlatform.EVENT,
     HmPlatform.LIGHT,
     HmPlatform.LOCK,
     HmPlatform.NUMBER,
     HmPlatform.SELECT,
     HmPlatform.SENSOR,
     HmPlatform.SIREN,
     HmPlatform.SWITCH,
@@ -468,7 +473,12 @@
     HmPlatform.HUB_BUTTON,
     HmPlatform.HUB_NUMBER,
     HmPlatform.HUB_SELECT,
     HmPlatform.HUB_SENSOR,
     HmPlatform.HUB_SWITCH,
     HmPlatform.HUB_TEXT,
 )
+
+ENTITY_EVENTS: Final = (
+    HmEventType.IMPULSE,
+    HmEventType.KEYPRESS,
+)
```

### Comparing `hahomematic-2023.7.3/hahomematic/decorators.py` & `hahomematic-2023.7.4/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/exceptions.py` & `hahomematic-2023.7.4/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/exporter.py` & `hahomematic-2023.7.4/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/hmcli.py` & `hahomematic-2023.7.4/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.4/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.4/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/light.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
         """
         if (
             self._e_device_operation_mode.value in (_DOM_RGB, _DOM_RGBW)
             and self.channel_no in (2, 3, 4)
         ) or (
             self._e_device_operation_mode.value == _DOM_TUNABLE_WHITE and self.channel_no in (3, 4)
         ):
-            return HmEntityUsage.ENTITY_NO_CREATE
+            return HmEntityUsage.NO_CREATE
         return self._attr_usage
 
     @value_property
     def effect_list(self) -> list[str] | None:
         """Return the list of supported effects."""
         return list(self._e_effect.value_list or ())
```

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.4/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/device.py` & `hahomematic-2023.7.4/hahomematic/platforms/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,32 +6,38 @@
 from dataclasses import dataclass
 from datetime import datetime
 import logging
 from typing import Any, Final
 
 from hahomematic import central_unit as hmcu, exporter as hmexp
 from hahomematic.const import (
+    ENTITY_EVENTS,
     EVENT_CONFIG_PENDING,
     EVENT_STICKY_UN_REACH,
     EVENT_UN_REACH,
     HM_AVAILABLE_FIRMWARE,
     HM_FIRMWARE,
     HM_FIRMWARE_UPDATABLE,
     HM_FIRMWARE_UPDATE_STATE,
     HM_SUBTYPE,
     HM_TYPE,
     HM_VIRTUAL_REMOTE_TYPES,
+    IDENTIFIER_SEPARATOR,
     INIT_DATETIME,
+    MANUFACTURER_EQ3,
+    MANUFACTURER_HB,
+    MANUFACTURER_MOEHLENHOFF,
     MAX_CACHE_AGE,
     NO_CACHE_ENTRY,
     PARAMSET_KEY_MASTER,
     PARAMSET_KEY_VALUES,
     RELEVANT_INIT_PARAMETERS,
     HmCallSource,
     HmDeviceFirmwareState,
+    HmEventType,
     HmForcedDeviceAvailability,
     HmInterface,
     HmProductGroup,
 )
 from hahomematic.exceptions import BaseHomematicException
 from hahomematic.platforms import custom as cep
 from hahomematic.platforms.custom import entity as hmce
@@ -65,18 +71,18 @@
             interface_id, device_address
         )
         _LOGGER.debug(
             "__INIT__: Initializing device: %s, %s",
             interface_id,
             device_address,
         )
+        self.custom_entities: Final[dict[str, hmce.CustomEntity]] = {}
         self.generic_entities: Final[dict[tuple[str, str], GenericEntity]] = {}
+        self.generic_events: Final[dict[tuple[str, str], GenericEvent]] = {}
         self.wrapper_entities: Final[dict[tuple[str, str], WrapperEntity]] = {}
-        self.custom_entities: Final[dict[str, hmce.CustomEntity]] = {}
-        self.events: Final[dict[tuple[str, str], GenericEvent]] = {}
         self._attr_last_update: datetime = INIT_DATETIME
         self._forced_availability: HmForcedDeviceAvailability = HmForcedDeviceAvailability.NOT_SET
         self._update_callbacks: Final[list[Callable]] = []
         self._firmware_update_callbacks: Final[list[Callable]] = []
         self._attr_device_type: Final = str(
             self.central.device_descriptions.get_device_parameter(
                 interface_id=interface_id,
@@ -87,20 +93,20 @@
         self._attr_sub_type: Final = str(
             central.device_descriptions.get_device_parameter(
                 interface_id=interface_id,
                 device_address=device_address,
                 parameter=HM_SUBTYPE,
             )
         )
+        self._attr_manufacturer = self._identify_manufacturer()
         self._attr_product_group: Final = self._identify_product_group()
         # marker if device will be created as custom entity
         self._has_custom_entity_definition: Final = cep.has_custom_entity_definition_by_device(
             device=self
         )
-
         self._attr_name: Final = get_device_name(
             central=central,
             device_address=device_address,
             device_type=self._attr_device_type,
         )
         self.value_cache: Final = ValueCache(device=self)
         self._attr_room: Final = central.device_details.get_room(device_address=device_address)
@@ -151,14 +157,22 @@
             self.central.device_descriptions.get_device_parameter(
                 interface_id=self._attr_interface_id,
                 device_address=self._attr_device_address,
                 parameter=HM_FIRMWARE_UPDATABLE,
             )
         )
 
+    def _identify_manufacturer(self) -> str:
+        """Identify the manufacturer of a device."""
+        if self.device_type.lower().startswith("hb"):
+            return MANUFACTURER_HB
+        if self.device_type.lower().startswith("alpha"):
+            return MANUFACTURER_MOEHLENHOFF
+        return MANUFACTURER_EQ3
+
     def _identify_product_group(self) -> HmProductGroup:
         """Identify the product group of the homematic device."""
         if self.interface == HmInterface.HMIP:
             l_device_type = self.device_type.lower()
             if l_device_type.startswith("hmipw"):
                 return HmProductGroup.HMIPW
             if l_device_type.startswith("hmip"):
@@ -217,14 +231,19 @@
 
     @config_property
     def firmware_update_state(self) -> HmDeviceFirmwareState:
         """Return the firmware update state of the device."""
         return self._attr_firmware_update_state
 
     @config_property
+    def identifier(self) -> str:
+        """Return the identifier of the device."""
+        return f"{self._attr_device_address}{IDENTIFIER_SEPARATOR}{self._attr_interface_id}"
+
+    @config_property
     def interface(self) -> str:
         """Return the interface of the device."""
         return self._attr_interface
 
     @config_property
     def interface_id(self) -> str:
         """Return the interface_id of the device."""
@@ -232,14 +251,19 @@
 
     @property
     def has_custom_entity_definition(self) -> bool:
         """Return if custom_entity definition is available for the device."""
         return self._has_custom_entity_definition
 
     @config_property
+    def manufacturer(self) -> str:
+        """Return the manufacturer of the device."""
+        return self._attr_manufacturer
+
+    @config_property
     def name(self) -> str:
         """Return the name of the device."""
         return self._attr_name
 
     @config_property
     def product_group(self) -> HmProductGroup:
         """Return the product group of the device."""
@@ -284,51 +308,51 @@
             self.register_update_callback(entity.update_entity)
         if isinstance(entity, WrapperEntity):
             self.wrapper_entities[(entity.channel_address, entity.parameter)] = entity
             self.register_update_callback(entity.update_entity)
         if isinstance(entity, hmce.CustomEntity):
             self.custom_entities[entity.unique_identifier] = entity
         if isinstance(entity, GenericEvent):
-            self.events[(entity.channel_address, entity.parameter)] = entity
+            self.generic_events[(entity.channel_address, entity.parameter)] = entity
 
     def remove_entity(self, entity: CallbackEntity) -> None:
         """Add a hm entity to a device."""
         if isinstance(entity, BaseEntity):
             self.central.remove_entity(entity=entity)
         if isinstance(entity, GenericEntity):
             del self.generic_entities[(entity.channel_address, entity.parameter)]
             self.unregister_update_callback(entity.update_entity)
         if isinstance(entity, WrapperEntity):
             del self.wrapper_entities[(entity.channel_address, entity.parameter)]
             self.unregister_update_callback(entity.update_entity)
         if isinstance(entity, hmce.CustomEntity):
             del self.custom_entities[entity.unique_identifier]
         if isinstance(entity, GenericEvent):
-            del self.events[(entity.channel_address, entity.parameter)]
+            del self.generic_events[(entity.channel_address, entity.parameter)]
         entity.remove_entity()
 
     def clear_collections(self) -> None:
         """Remove entities from collections and central."""
-        for event in list(self.events.values()):
+        for event in list(self.generic_events.values()):
             self.remove_entity(event)
-        self.events.clear()
+        self.generic_events.clear()
 
         for entity in list(self.generic_entities.values()):
             self.remove_entity(entity)
         self.generic_entities.clear()
 
         for custom_entity in list(self.custom_entities.values()):
             self.remove_entity(custom_entity)
         self.custom_entities.clear()
 
         for wrapper_entity in list(self.wrapper_entities.values()):
             self.remove_entity(wrapper_entity)
         self.wrapper_entities.clear()
 
-        self.events.clear()
+        self.generic_events.clear()
 
     def register_update_callback(self, update_callback: Callable) -> None:
         """Register update callback."""
         if callable(update_callback) and update_callback not in self._update_callbacks:
             self._update_callbacks.append(update_callback)
 
     def unregister_update_callback(self, update_callback: Callable) -> None:
@@ -356,18 +380,35 @@
         """Return all entities of a device."""
         all_entities: list[hmce.CustomEntity | GenericEntity | WrapperEntity] = []
         all_entities.extend(self.custom_entities.values())
         all_entities.extend(self.generic_entities.values())
         all_entities.extend(self.wrapper_entities.values())
         return all_entities
 
+    def get_channel_events(self, event_type: HmEventType) -> dict[int, list[GenericEvent]]:
+        """Return a list of specific events of a channel."""
+        event_dict: dict[int, list[GenericEvent]] = {}
+        if event_type not in ENTITY_EVENTS:
+            return event_dict
+        for event in self.generic_events.values():
+            if event.event_type == event_type and event.channel_no is not None:
+                if event.channel_no not in event_dict:
+                    event_dict[event.channel_no] = []
+                event_dict[event.channel_no].append(event)
+
+        return event_dict
+
     def get_generic_entity(self, channel_address: str, parameter: str) -> GenericEntity | None:
         """Return an entity from device."""
         return self.generic_entities.get((channel_address, parameter))
 
+    def get_generic_event(self, channel_address: str, parameter: str) -> GenericEvent | None:
+        """Return a generic event from device."""
+        return self.generic_events.get((channel_address, parameter))
+
     def set_forced_availability(self, forced_availability: HmForcedDeviceAvailability) -> None:
         """Set the availability of the device."""
         if self._forced_availability != forced_availability:
             self._forced_availability = forced_availability
             for entity in self.generic_entities.values():
                 entity.update_entity()
 
@@ -413,15 +454,15 @@
 
         return update_result
 
     async def load_value_cache(self) -> None:
         """Init the parameter cache."""
         if len(self.generic_entities) > 0:
             await self.value_cache.init_base_entities()
-        if len(self.events) > 0:
+        if len(self.generic_events) > 0:
             await self.value_cache.init_readable_events()
         _LOGGER.debug(
             "INIT_DATA: Skipping load_data, missing entities for %s",
             self._attr_device_address,
         )
 
     async def reload_paramset_descriptions(self) -> None:
@@ -455,15 +496,15 @@
         return (
             f"address: {self._attr_device_address}, "
             f"type: {len(self._attr_device_type)}, "
             f"name: {self._attr_name}, "
             f"generic_entities: {len(self.generic_entities)}, "
             f"custom_entities: {len(self.custom_entities)}, "
             f"wrapper_entities: {len(self.wrapper_entities)}, "
-            f"events: {len(self.events)}"
+            f"events: {len(self.generic_events)}"
         )
 
 
 class ValueCache:
     """A Cache to temporaily stored values."""
 
     _NO_VALUE_CACHE_ENTRY: Final = "NO_VALUE_CACHE_ENTRY"
@@ -525,15 +566,15 @@
                 self._attr_device.device_address,
                 bhe,
             )
 
     def _get_readable_events(self) -> set[GenericEvent]:
         """Get readable events."""
         events: list[GenericEvent] = []
-        for event in self._attr_device.events.values():
+        for event in self._attr_device.generic_events.values():
             if event.is_readable:
                 events.append(event)
         return set(events)
 
     async def get_value(
         self,
         channel_address: str,
```

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/entity.py` & `hahomematic-2023.7.4/hahomematic/platforms/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 )
 from hahomematic.platforms import device as hmd
 from hahomematic.platforms.support import (
     EntityNameData,
     PayloadMixin,
     config_property,
     convert_value,
+    generate_channel_unique_identifier,
     value_property,
 )
 
 HM_EVENT_DATA_SCHEMA = vol.Schema(
     {
         vol.Required(ATTR_ADDRESS): str,
         vol.Required(ATTR_CHANNEL_NO): int,
@@ -134,18 +135,18 @@
             self._remove_callbacks.append(remove_callback)
 
     def unregister_remove_callback(self, remove_callback: Callable) -> None:
         """Unregister the remove callback."""
         if remove_callback in self._remove_callbacks:
             self._remove_callbacks.remove(remove_callback)
 
-    def update_entity(self, *args: Any) -> None:
+    def update_entity(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated."""
         for _callback in self._update_callbacks:
-            _callback(*args)
+            _callback(*args, **kwargs)
 
     def remove_entity(self, *args: Any) -> None:
         """Do what is needed when the entity has been removed."""
         for _callback in self._remove_callbacks:
             _callback(*args)
 
 
@@ -163,26 +164,30 @@
         PayloadMixin.__init__(self)
         super().__init__(unique_identifier=unique_identifier)
         self.device: Final = device
         self._attr_channel_no: Final = channel_no
         self._attr_channel_address: Final[str] = hms.get_channel_address(
             device_address=device.device_address, channel_no=channel_no
         )
+        self._attr_channel_unique_identifier: Final = generate_channel_unique_identifier(
+            central=device.central, address=self._attr_channel_address
+        )
         self._attr_is_in_multiple_channels: Final = is_in_multiple_channels
         self._central: Final[hmcu.CentralUnit] = device.central
         self._channel_type: Final = str(device.channels[self._attr_channel_address].type)
         self._attr_function: Final = self._central.device_details.get_function_text(
             address=self._attr_channel_address
         )
         self._client: Final[hmcl.Client] = device.central.get_client(
             interface_id=device.interface_id
         )
 
         self._attr_usage: HmEntityUsage = self._get_entity_usage()
         entity_name_data: Final = self._get_entity_name()
+        self._attr_channel_name: Final = entity_name_data.channel_name
         self._attr_full_name: Final = entity_name_data.full_name
         self._attr_name: Final = entity_name_data.entity_name
 
     @property
     def address_path(self) -> str:
         """Return the address pass of the entity."""
         return f"{self._attr_platform}/{self.device.interface_id}/{self._attr_unique_identifier}/"
@@ -194,19 +199,29 @@
 
     @config_property
     def channel_address(self) -> str:
         """Return the channel_address of the entity."""
         return self._attr_channel_address
 
     @config_property
+    def channel_name(self) -> str:
+        """Return the channel_name of the entity."""
+        return self._attr_channel_name
+
+    @config_property
     def channel_no(self) -> int | None:
         """Return the channel_no of the entity."""
         return self._attr_channel_no
 
     @config_property
+    def channel_unique_identifier(self) -> str:
+        """Return the channel_unique_identifier of the entity."""
+        return self._attr_channel_unique_identifier
+
+    @config_property
     def function(self) -> str | None:
         """Return the function of the entity."""
         return self._attr_function
 
     @config_property
     def full_name(self) -> str:
         """Return the full name of the entity."""
@@ -227,17 +242,17 @@
         """Return the entity usage."""
         return self._attr_usage
 
     def set_usage(self, usage: HmEntityUsage) -> None:
         """Set the entity usage."""
         self._attr_usage = usage
 
-    def update_entity(self, *args: Any) -> None:
+    def update_entity(self, *args: Any, **kwargs: Any) -> None:
         """Do what is needed when the value of the entity has been updated."""
-        super().update_entity(*args)
+        super().update_entity(*args, **kwargs)
         self._central.fire_entity_data_event_callback(
             interface_id=self.device.interface_id, entity=self
         )
 
     @abstractmethod
     async def load_entity_value(
         self, call_source: HmCallSource, max_age_seconds: int = MAX_CACHE_AGE
```

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/event.py` & `hahomematic-2023.7.4/hahomematic/platforms/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Functions for event creation."""
 from __future__ import annotations
 
 import logging
 from typing import Any
 
+from hahomematic import support as hms
 from hahomematic.const import (
     CLICK_EVENTS,
     DEVICE_ERROR_EVENTS,
+    ENTITY_EVENTS,
     HM_OPERATIONS,
     IMPULSE_EVENTS,
     OPERATION_EVENT,
     PARAMSET_KEY_VALUES,
     HmEntityUsage,
     HmEventType,
     HmPlatform,
@@ -52,23 +54,25 @@
         )
 
     @config_property
     def usage(self) -> HmEntityUsage:
         """Return the entity usage."""
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._attr_usage
-        return HmEntityUsage.EVENT if force_enabled else HmEntityUsage.ENTITY_NO_CREATE
+        return HmEntityUsage.EVENT if force_enabled else HmEntityUsage.NO_CREATE
 
     @config_property
     def event_type(self) -> HmEventType:
         """Return the event_type of the event."""
         return self._attr_event_type
 
     def event(self, value: Any) -> None:
         """Handle event for which this handler has subscribed."""
+        if self.event_type in ENTITY_EVENTS:
+            self.update_entity(parameter=self.parameter.lower())
         self.fire_event(value)
 
     def fire_event(self, value: Any) -> None:
         """Do what is needed to fire an event."""
         self._central.fire_ha_event_callback(
             event_type=self.event_type, event_data=self.get_event_data(value=value)
         )
@@ -128,14 +132,26 @@
     _attr_event_type = HmEventType.IMPULSE
 
 
 def create_event_and_append_to_device(
     device: hmd.HmDevice, channel_address: str, parameter: str, parameter_data: dict[str, Any]
 ) -> None:
     """Create action event entity."""
+    if device.central.parameter_visibility.parameter_is_ignored(
+        device_type=device.device_type,
+        channel_no=hms.get_channel_no(address=channel_address),
+        paramset_key=PARAMSET_KEY_VALUES,
+        parameter=parameter,
+    ):
+        _LOGGER.debug(
+            "create_event_and_append_to_device: Ignoring parameter: %s [%s]",
+            parameter,
+            channel_address,
+        )
+        return
     unique_identifier = generate_unique_identifier(
         central=device.central,
         address=channel_address,
         parameter=parameter,
         prefix=f"event_{device.central.name}",
     )
```

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.wrapped: bool = False
 
     @config_property
     def usage(self) -> HmEntityUsage:
         """Return the entity usage."""
         if (force_enabled := self._enabled_by_channel_operation_mode) is None:
             return self._attr_usage
-        return HmEntityUsage.ENTITY if force_enabled else HmEntityUsage.ENTITY_NO_CREATE
+        return HmEntityUsage.ENTITY if force_enabled else HmEntityUsage.NO_CREATE
 
     def event(self, value: Any) -> None:
         """Handle event for which this entity has subscribed."""
         old_value = self._attr_value
         new_value = self._convert_value(value)
         if self._attr_value == new_value:
             return
@@ -139,18 +139,18 @@
         """Generate the usage for the entity."""
         if self._central.parameter_visibility.parameter_is_hidden(
             device_type=self.device.device_type,
             channel_no=self.channel_no,
             paramset_key=self._attr_paramset_key,
             parameter=self._attr_parameter,
         ):
-            return HmEntityUsage.ENTITY_NO_CREATE
+            return HmEntityUsage.NO_CREATE
 
         return (
-            HmEntityUsage.ENTITY_NO_CREATE
+            HmEntityUsage.NO_CREATE
             if self.device.has_custom_entity_definition
             else HmEntityUsage.ENTITY
         )
 
     def is_state_change(self, value: hme.ParameterT) -> bool:
         """
         Check if the state/value changes.
@@ -182,15 +182,15 @@
             is_in_multiple_channels=wrapped_entity.is_in_multiple_channels,
         )
         self._attr_platform = new_platform
         # use callbacks from wrapped entity
         self._update_callbacks = wrapped_entity._update_callbacks
         self._remove_callbacks = wrapped_entity._remove_callbacks
         # hide wrapped entity from HA
-        wrapped_entity.set_usage(HmEntityUsage.ENTITY_NO_CREATE)
+        wrapped_entity.set_usage(HmEntityUsage.NO_CREATE)
         wrapped_entity.wrapped = True
 
     async def load_entity_value(
         self, call_source: HmCallSource, max_age_seconds: int = MAX_CACHE_AGE
     ) -> None:
         """Init the entity data."""
         await self._wrapped_entity.load_entity_value(
```

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.4/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.4/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/support.py` & `hahomematic-2023.7.4/hahomematic/platforms/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,26 @@
         self, device_name: str, channel_name: str, parameter_name: str | None = None
     ) -> None:
         """Init the EntityNameData class."""
         self._device_name = device_name
         self._channel_name = channel_name
         self._parameter_name = parameter_name
 
+    @property
+    def channel_name(self) -> str:
+        """Return the channel_name of the entity only name."""
+        if (
+            self._device_name
+            and self._channel_name
+            and self._channel_name.startswith(self._device_name)
+        ):
+            return self._channel_name.replace(self._device_name, "").strip()
+
+        return self._channel_name.strip()
+
     @staticmethod
     def empty() -> EntityNameData:
         """Return an empty EntityNameData."""
         return EntityNameData(device_name="", channel_name="")
 
     @property
     def entity_name(self) -> str | None:
@@ -280,20 +292,19 @@
     if channel_name := _get_base_name_from_channel_or_device(
         central=central,
         device=device,
         channel_no=channel_no,
     ):
         p_name = parameter.title().replace("_", " ")
         if _check_channel_name_with_channel_no(name=channel_name):
-            d_name = channel_name.split(":")[0]
-            c_name = "" if channel_no in (0, None) else f" Channel {channel_no}"
+            c_name = "" if channel_no in (0, None) else f" ch{channel_no}"
             event_name = EntityNameData(
                 device_name=device.name,
-                channel_name=d_name,
-                parameter_name=f"{c_name} {p_name}",
+                channel_name=c_name,
+                parameter_name=p_name,
             )
         else:
             event_name = EntityNameData(
                 device_name=device.name,
                 channel_name=channel_name,
                 parameter_name=p_name,
             )
@@ -365,14 +376,25 @@
         or address.startswith("INT000")
         or address.split(":")[0] in HM_VIRTUAL_REMOTE_ADDRESSES
     ):
         return f"{central.config.central_id}_{unique_identifier}".lower()
     return f"{unique_identifier}".lower()
 
 
+def generate_channel_unique_identifier(
+    central: hmcu.CentralUnit,
+    address: str,
+) -> str:
+    """Build unique identifier for a channel from address."""
+    unique_identifier = address.replace(":", "_").replace("-", "_")
+    if address.split(":")[0] in HM_VIRTUAL_REMOTE_ADDRESSES:
+        return f"{central.config.central_id}_{unique_identifier}".lower()
+    return unique_identifier.lower()
+
+
 def _get_base_name_from_channel_or_device(
     central: hmcu.CentralUnit,
     device: hmd.HmDevice,
     channel_no: int | None,
 ) -> str | None:
     """Get the name from channel if it's not default, otherwise from device."""
     channel_address = hms.get_channel_address(
```

### Comparing `hahomematic-2023.7.3/hahomematic/platforms/update.py` & `hahomematic-2023.7.4/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.4/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.4/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.4/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/support.py` & `hahomematic-2023.7.4/hahomematic/support.py`

 * *Files 14% similar despite different names*

```diff
@@ -184,34 +184,61 @@
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return int(sock.getsockname()[1])
 
 
 def element_matches_key(
     search_elements: str | Collection[str],
     compare_with: str | None,
+    search_key: str | None = None,
     do_wildcard_search: bool = True,
 ) -> bool:
-    """Return if collection element is key."""
-    if compare_with is None:
+    """
+    Return if collection element is key.
+
+    A set search_key assumes that search_elements is initially a dict,
+    and it tries to identify a matching key (wildcard) in the dict keys to use it on the dict.
+    """
+    if compare_with is None or not search_elements:
         return False
 
     if isinstance(search_elements, str):
         if do_wildcard_search:
-            return compare_with.lower().startswith(search_elements.lower())
+            return compare_with.lower().startswith(
+                search_elements.lower()
+            )  # or search_elements.lower().startswith(compare_with.lower())
         return compare_with.lower() == search_elements.lower()
     if isinstance(search_elements, Collection):
+        if isinstance(search_elements, dict):
+            if (
+                match_key := _get_search_key(
+                    search_elements=search_elements, search_key=search_key
+                )
+                if search_key
+                else None
+            ):
+                if (elements := search_elements.get(match_key)) is None:
+                    return False
+                search_elements = elements
         for element in search_elements:
             if do_wildcard_search:
                 if compare_with.lower().startswith(element.lower()):
                     return True
             elif compare_with.lower() == element.lower():
                 return True
     return False
 
 
+def _get_search_key(search_elements: Collection[str], search_key: str) -> str | None:
+    """Search for a matching key in a collection."""
+    for element in search_elements:
+        if search_key.startswith(element):
+            return element
+    return None
+
+
 @dataclass
 class HubData:
     """Dataclass for hub entities."""
 
     name: str
 
 
@@ -252,7 +279,13 @@
 
 
 @dataclass
 class Channel:
     """dataclass for a device channel."""
 
     type: str
+    address: str
+
+    @property
+    def no(self) -> int | None:
+        """Return the channel no."""
+        return get_channel_no(self.address)
```

### Comparing `hahomematic-2023.7.3/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.4/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.4/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.4/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.3/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.4/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.3/pyproject.toml` & `hahomematic-2023.7.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.3"
+version     = "2023.7.4"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

