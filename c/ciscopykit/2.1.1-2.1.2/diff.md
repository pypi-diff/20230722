# Comparing `tmp/ciscopykit-2.1.1.tar.gz` & `tmp/ciscopykit-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-2.1.1.tar", last modified: Fri Jul 21 05:08:19 2023, max compression
+gzip compressed data, was "ciscopykit-2.1.2.tar", last modified: Fri Jul 21 23:05:47 2023, max compression
```

## Comparing `ciscopykit-2.1.1.tar` & `ciscopykit-2.1.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.117448 ciscopykit-2.1.1/ciscopykit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.117448 ciscopykit-2.1.1/ciscopykit/help/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/help/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.117448 ciscopykit-2.1.1/ciscopykit/lan_security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/dhcp_snooping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/dynamic_arp_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/stp_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/switchport_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/lan_security/vlan_security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.117448 ciscopykit-2.1.1/ciscopykit/routing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/routing/dynamic_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/routing/static_routing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/ciscopykit/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/services/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/services/dhcp_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/services/pat_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/ciscopykit/switch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/switch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/switch/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/switch/l2_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/switch/l3_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/switch/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/ciscopykit/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/templates/generate_router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/ciscopykit/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/vlan/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/ciscopykit/vlan/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:08:19.117448 ciscopykit-2.1.1/ciscopykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-21 05:08:19.000000 ciscopykit-2.1.1/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 05:08:19.000000 ciscopykit-2.1.1/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:08:19.000000 ciscopykit-2.1.1/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-21 05:08:19.000000 ciscopykit-2.1.1/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 05:08:19.000000 ciscopykit-2.1.1/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 05:08:19.000000 ciscopykit-2.1.1/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:08:19.121448 ciscopykit-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-21 05:08:03.000000 ciscopykit-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.639316 ciscopykit-2.1.2/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.639316 ciscopykit-2.1.2/ciscopykit/help/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/help/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.639316 ciscopykit-2.1.2/ciscopykit/lan_security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/dhcp_snooping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/dynamic_arp_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/stp_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/switchport_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/lan_security/vlan_security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/ciscopykit/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/routing/dynamic_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/routing/static_routing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/ciscopykit/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/services/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/services/dhcp_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/services/pat_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/ciscopykit/switch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/switch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/switch/l2_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/switch/l3_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/switch/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/ciscopykit/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/vlan/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/ciscopykit/vlan/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:05:47.639316 ciscopykit-2.1.2/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-21 23:05:47.000000 ciscopykit-2.1.2/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 23:05:47.000000 ciscopykit-2.1.2/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 23:05:47.000000 ciscopykit-2.1.2/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-21 23:05:47.000000 ciscopykit-2.1.2/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 23:05:47.000000 ciscopykit-2.1.2/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 23:05:47.000000 ciscopykit-2.1.2/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 23:05:47.643316 ciscopykit-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-21 23:05:32.000000 ciscopykit-2.1.2/setup.py
```

### Comparing `ciscopykit-2.1.1/LICENSE.md` & `ciscopykit-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/PKG-INFO` & `ciscopykit-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 2.1.1
+Version: 2.1.2
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-2.1.1/README.md` & `ciscopykit-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/app.py` & `ciscopykit-2.1.2/ciscopykit/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/device.py` & `ciscopykit-2.1.2/ciscopykit/device.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/entry_point.py` & `ciscopykit-2.1.2/ciscopykit/entry_point.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/interface.py` & `ciscopykit-2.1.2/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/lan_security/app.py` & `ciscopykit-2.1.2/ciscopykit/lan_security/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/lan_security/dhcp_snooping.py` & `ciscopykit-2.1.2/ciscopykit/lan_security/dhcp_snooping.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/lan_security/dynamic_arp_inspection.py` & `ciscopykit-2.1.2/ciscopykit/lan_security/dynamic_arp_inspection.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/lan_security/stp_security.py` & `ciscopykit-2.1.2/ciscopykit/lan_security/stp_security.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/lan_security/switchport_security.py` & `ciscopykit-2.1.2/ciscopykit/lan_security/switchport_security.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/lan_security/vlan_security.py` & `ciscopykit-2.1.2/ciscopykit/lan_security/vlan_security.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/routing/static_routing.py` & `ciscopykit-2.1.2/ciscopykit/routing/static_routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 This module provides functions to configure static routes 
 and route redistribution for Cisco devices.
 
 Functions:
 - configure_static_route(destination, next_hop, administrative_distance=1): Configures a static route on the device.
 - configure_default_route(next_hop, exit_interface): Configures a default route on the device.
 - configure_route_redistribution(source_protocol, destination_protocol): Configures route redistribution between routing protocols.
-
 """
 
 import ipaddress
 
 
 def configure_static_route(destination, next_hop, administrative_distance=1):
     """
```

### Comparing `ciscopykit-2.1.1/ciscopykit/services/app.py` & `ciscopykit-2.1.2/ciscopykit/services/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/services/dhcp_service.py` & `ciscopykit-2.1.2/ciscopykit/services/dhcp_service.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/services/pat_service.py` & `ciscopykit-2.1.2/ciscopykit/services/pat_service.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/switch/app.py` & `ciscopykit-2.1.2/ciscopykit/switch/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/switch/l3_switch.py` & `ciscopykit-2.1.2/ciscopykit/switch/l3_switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/switch/switch.py` & `ciscopykit-2.1.2/ciscopykit/switch/switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/templates/generate_router_config.py` & `ciscopykit-2.1.2/ciscopykit/templates/generate_router_config.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/vlan/app.py` & `ciscopykit-2.1.2/ciscopykit/vlan/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit/vlan/vlan.py` & `ciscopykit-2.1.2/ciscopykit/vlan/vlan.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/ciscopykit.egg-info/PKG-INFO` & `ciscopykit-2.1.2/ciscopykit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 2.1.1
+Version: 2.1.2
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-2.1.1/ciscopykit.egg-info/SOURCES.txt` & `ciscopykit-2.1.2/ciscopykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ciscopykit-2.1.1/setup.py` & `ciscopykit-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='2.1.1',
+    version='2.1.2',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
     description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
     long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
     url='https://github.com/Vincent-de-Torres-Portfolio/ciscopykit',
     packages=find_packages(),
     classifiers=[
```

