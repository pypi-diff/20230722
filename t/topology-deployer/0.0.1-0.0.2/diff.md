# Comparing `tmp/topology-deployer-0.0.1.tar.gz` & `tmp/topology-deployer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topology-deployer-0.0.1.tar", last modified: Wed Jul 19 03:39:41 2023, max compression
+gzip compressed data, was "topology-deployer-0.0.2.tar", last modified: Sat Jul 22 03:58:01 2023, max compression
```

## Comparing `topology-deployer-0.0.1.tar` & `topology-deployer-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:39:41.037991 topology-deployer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-19 03:39:41.037991 topology-deployer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:39:41.037991 topology-deployer-0.0.1/deployer/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/nat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/deployer/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 03:39:41.037991 topology-deployer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-19 03:39:28.000000 topology-deployer-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 03:39:41.037991 topology-deployer-0.0.1/topology_deployer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-19 03:39:41.000000 topology-deployer-0.0.1/topology_deployer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-19 03:39:41.000000 topology-deployer-0.0.1/topology_deployer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 03:39:41.000000 topology-deployer-0.0.1/topology_deployer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 03:39:41.000000 topology-deployer-0.0.1/topology_deployer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-19 03:39:41.000000 topology-deployer-0.0.1/topology_deployer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 03:39:41.000000 topology-deployer-0.0.1/topology_deployer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 03:58:01.233827 topology-deployer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-22 03:58:01.233827 topology-deployer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 03:58:01.229827 topology-deployer-0.0.2/deployer/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/nat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/deployer/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 03:58:01.233827 topology-deployer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-22 03:57:49.000000 topology-deployer-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 03:58:01.229827 topology-deployer-0.0.2/topology_deployer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-22 03:58:01.000000 topology-deployer-0.0.2/topology_deployer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-22 03:58:01.000000 topology-deployer-0.0.2/topology_deployer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 03:58:01.000000 topology-deployer-0.0.2/topology_deployer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-22 03:58:01.000000 topology-deployer-0.0.2/topology_deployer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-22 03:58:01.000000 topology-deployer-0.0.2/topology_deployer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 03:58:01.000000 topology-deployer-0.0.2/topology_deployer.egg-info/top_level.txt
```

### Comparing `topology-deployer-0.0.1/PKG-INFO` & `topology-deployer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topology-deployer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python tool to deploy topology defined in a json config
 Home-page: https://github.com/vpatel95/libvirt-topology
 Author: Ved Patel
 Project-URL: Bug Tracker, https://github.com/vpatel95/libvirt-topology/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `topology-deployer-0.0.1/README.md` & `topology-deployer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `topology-deployer-0.0.1/deployer/globals.py` & `topology-deployer-0.0.2/deployer/globals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from pathlib import Path
 
+OP_CREATE = 1
+OP_DELETE = 2
+
+OP = OP_CREATE
 DRY_RUN = False
 NO_NETWORK = False
 NO_VM = False
 RECREATE_NW = False
 PRINT_NETWORK = False
 PRINT_VM = False
```

### Comparing `topology-deployer-0.0.1/deployer/nat_utils.py` & `topology-deployer-0.0.2/deployer/nat_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,7 +56,37 @@
     ExecuteCommand("sudo iptables -t filter -A INPUT -i "
                    "{} -p tcp -m tcp -m multiport --dports 53,67 -j ACCEPT".format(name))
     ExecuteCommand("sudo iptables -t filter -A FORWARD -d {} -o {} -j ACCEPT".format(nw4, name))
     ExecuteCommand("sudo iptables -t filter -A FORWARD -s {} -i {} -j ACCEPT".format(nw4, name))
     ExecuteCommand("sudo iptables -t filter -A FORWARD -i {} -j ACCEPT".format(name))
     ExecuteCommand("sudo iptables -t filter -A FORWARD -o {} -j ACCEPT".format(name))
     ExecuteCommand("sudo sh -c 'iptables-save > /etc/iptables/rules.v4'")
+
+def DelLinuxBridge(name: str) -> None:
+    dummy_intf = "{}-nic".format(name)
+    ExecuteCommand("sudo ip link set dev {} down".format(dummy_intf))
+    ExecuteCommand("sudo ip link set dev {} down".format(name))
+    ExecuteCommand("sudo ip link del {}".format(dummy_intf))
+    ExecuteCommand("sudo ip link del {}".format(name))
+
+def DelIptableRules(name: str, nw4: str) -> None:
+    ExecuteCommand("sudo iptables -t mangle -D POSTROUTING "
+                   "-o {} -p udp -m udp --dport 68 -j CHECKSUM --checksum-fill".format(name))
+    ExecuteCommand("sudo iptables -t nat -D POSTROUTING "
+                   "-s {} -d 224.0.0.0/24 -j RETURN".format(nw4))
+    ExecuteCommand("sudo iptables -t nat -D POSTROUTING "
+                   "-s {} -d 255.255.255.255/32 -j RETURN".format(nw4))
+    ExecuteCommand("sudo iptables -t nat -D POSTROUTING "
+                   "-s {} ! -d {} -p tcp -j MASQUERADE --to-ports 1024-65535".format(nw4, nw4))
+    ExecuteCommand("sudo iptables -t nat -D POSTROUTING "
+                   "-s {} ! -d {} -p udp -j MASQUERADE --to-ports 1024-65535".format(nw4, nw4))
+    ExecuteCommand("sudo iptables -t nat -D POSTROUTING -s {} ! -d {} -j MASQUERADE".format(nw4, nw4))
+    ExecuteCommand("sudo iptables -t filter -D INPUT "
+                   "-i {} -p udp -m udp -m multiport --dports 53,67 -j ACCEPT".format(name))
+    ExecuteCommand("sudo iptables -t filter -D INPUT -i "
+                   "{} -p tcp -m tcp -m multiport --dports 53,67 -j ACCEPT".format(name))
+    ExecuteCommand("sudo iptables -t filter -D FORWARD -d {} -o {} -j ACCEPT".format(nw4, name))
+    ExecuteCommand("sudo iptables -t filter -D FORWARD -s {} -i {} -j ACCEPT".format(nw4, name))
+    ExecuteCommand("sudo iptables -t filter -D FORWARD -i {} -j ACCEPT".format(name))
+    ExecuteCommand("sudo iptables -t filter -D FORWARD -o {} -j ACCEPT".format(name))
+    ExecuteCommand("sudo sh -c 'iptables-save > /etc/iptables/rules.v4'")
+    pass
```

### Comparing `topology-deployer-0.0.1/deployer/network.py` & `topology-deployer-0.0.2/deployer/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import sys
 from xml.dom import minidom
 import xml.etree.cElementTree as ET
 
 import deployer.globals as globals
 from .globals import LIBVIRT_QEMU_NW, NAT_NW_BASE
-from .nat_utils import AddIptableRules, AddLinuxBridge, CheckForwarding
+from .nat_utils import AddIptableRules, AddLinuxBridge, CheckForwarding, DelIptableRules, DelLinuxBridge
 from .utils import ExecuteCommand
 
 class Network:
     topology_ = None
     type_ = ""
     name_ = ""
     ip4_ = None
@@ -142,14 +142,35 @@
         cmd = "sudo virsh net-define {}".format(nw_cfg_file)
         ExecuteCommand(cmd)
         cmd = "sudo virsh net-start {}".format(self.name_)
         ExecuteCommand(cmd)
         cmd = "sudo virsh net-autostart {}".format(self.name_)
         ExecuteCommand(cmd)
 
+    def __delete_nat_network(self):
+        DelIptableRules(self.name_, str(self.network4_))
+        DelLinuxBridge(self.name_)
+        NAT_NW_BASE.joinpath(self.name_).rmdir()
+        pass
+
+    def __delete_libvirt_network(self):
+        cmd = "sudo virsh net-destroy {}".format(self.name_)
+        ExecuteCommand(cmd)
+        cmd = "sudo virsh net-undefine {}".format(self.name_)
+        ExecuteCommand(cmd)
+
+    def Delete(self):
+        if self.type_ == "nat":
+            self.__delete_nat_network()
+        elif self.type_ in ["isolated","management"]:
+            self.__delete_libvirt_network()
+        else:
+            logging.error("Unknown network type {}".format(self.type_))
+            sys.exit(1)
+
 
     def Create(self):
         if self.type_ == "nat":
             self.__create_nat_network()
         elif self.type_ == "isolated":
             self.__create_isolated_network()
         elif self.type_ == "management":
```

### Comparing `topology-deployer-0.0.1/deployer/topology.py` & `topology-deployer-0.0.2/deployer/topology.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import sys
 
 import deployer.globals as globals
 # from .config import NO_NETWORK, NO_VM, PRINT_NETWORK, PRINT_VM
+from .globals import OP_CREATE, OP_DELETE
 from .network import Network
 from .virtual_machine import VirtualMachine
 
 class Topology:
     supported_network_types_ = ["nat", "isolated", "management"]
     def __new__(cls):
         if not hasattr(cls, 'instance'):
@@ -21,25 +22,18 @@
         if self.config is None:
             print("Error parsing config file")
             exit(1)
 
         self.networks = {}
         self.vms = {}
 
-        if not globals.NO_NETWORK:
-            self.CreateNetworks()
-
-        if not globals.NO_VM:
-            self.CreateVms()
-
-        if globals.PRINT_NETWORK:
-            self.PrintNetworks()
-
-        if globals.PRINT_VM:
-            self.PrintVms()
+        if globals.OP == OP_CREATE:
+            self.__create()
+        else:
+            self.__delete()
 
     def __is_nw_type_valid(self, nw_type: str) -> bool:
         return nw_type in self.supported_network_types_
 
     def __parse_networks(self):
         nw_config = self.config.get("networks", {})
         if nw_config:
@@ -49,42 +43,74 @@
                     sys.exit(1)
                 for nw in nw_config[nw_type]:
                     self.networks[nw["name"]] = Network(nw_type, nw, self)
         else:
             logging.critical("No network config found. Exiting")
             sys.exit(1)
 
-    def GetNetwork(self, name):
-        return self.networks.get(name, None)
-
-    def GetNetworkType(self, name):
-        if self.GetNetwork(name) is not None:
-            return self.networks[name].type_
-        return ""
-
     def __parse_vms(self):
         vms_config = self.config.get("vms", [])
         if vms_config:
             for vm_conf in vms_config:
                 if vm_conf is {}:
                     continue
                 self.vms[vm_conf["name"]] = VirtualMachine(vm_conf, self)
 
+    def __delete(self):
+        if not globals.NO_VM:
+            self.__delete_vms()
+
+        if not globals.NO_NETWORK:
+            self.__delete_networks()
+
+    def __delete_networks(self):
+        self.__parse_networks()
+        for _, nw in self.networks.items():
+            nw.Delete()
+        pass
+
+    def __delete_vms(self):
+        self.__parse_vms()
+        for _, vm in self.vms.items():
+            vm.Delete()
+
+    def __create(self):
+        if not globals.NO_NETWORK:
+            self.__create_networks()
+
+        if not globals.NO_VM:
+            self.__create_vms()
+
+        if globals.PRINT_NETWORK:
+            self.PrintNetworks()
+
+        if globals.PRINT_VM:
+            self.PrintVms()
+
+    def __create_networks(self):
+        self.__parse_networks()
+        for _, nw in self.networks.items():
+            nw.Create()
+
+    def __create_vms(self):
+        self.__parse_vms()
+        for _, vm in self.vms.items():
+            vm.Create()
+
+    def GetNetwork(self, name):
+        return self.networks.get(name, None)
+
+    def GetNetworkType(self, name):
+        if self.GetNetwork(name) is not None:
+            return self.networks[name].type_
+        return ""
+
     def PrintNetworks(self):
         for name, nw in self.networks.items():
             print("Network : {}".format(name))
             print(nw.ToString())
 
     def PrintVms(self):
         for name, vm in self.vms.items():
             print("Vm : {}".format(name))
             print(vm.ToString())
 
-    def CreateNetworks(self):
-        self.__parse_networks()
-        for _, nw in self.networks.items():
-            nw.Create()
-
-    def CreateVms(self):
-        self.__parse_vms()
-        for _, vm in self.vms.items():
-            vm.Create()
```

### Comparing `topology-deployer-0.0.1/deployer/utils.py` & `topology-deployer-0.0.2/deployer/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,52 @@
 import logging
 import shlex
 import subprocess
 import sys
 
 # from .config import DRY_RUN, NO_NETWORK, NO_VM, PRINT_NETWORK, PRINT_VM
 import deployer.globals as globals
+from .globals import OP_CREATE, OP_DELETE
 
 
 def ProcessArguments() -> str:
     parser = argparse.ArgumentParser(description="Parse topology config")
     parser.add_argument("-c", "--config", required=True)
     parser.add_argument("-l", "--log", type=str, choices=["DEBUG", "INFO",
                                                           "WARNING", "ERROR",
                                                           "CRITICAL"])
     parser.add_argument("--dry-run", action="store_true")
 
-    skip_operation = parser.add_mutually_exclusive_group()
-    skip_operation.add_argument("--no-network", action="store_true")
-    skip_operation.add_argument("--no-vm", action="store_true")
+    parser.add_argument("-o", "--operation", type=str, required=True,
+                        choices=["create", "delete", "CREATE", "DELETE"])
 
     parser.add_argument("--recreate-nw", action="store_true")
     parser.add_argument("--print-nw", action="store_true")
     parser.add_argument("--print-vm", action="store_true")
 
+    skip_operation = parser.add_mutually_exclusive_group()
+    skip_operation.add_argument("--no-network", action="store_true")
+    skip_operation.add_argument("--no-vm", action="store_true")
+
     args = parser.parse_args()
 
     if args.log:
         log_level = getattr(logging, args.log.upper(), None)
         if not isinstance(log_level, int):
             raise ValueError("Invalid log level: {}".format(args.log))
         logging.basicConfig(level=log_level)
 
     if args.dry_run:
         globals.DRY_RUN = args.dry_run
 
+    if args.operation.upper() == "CREATE":
+        globals.OP = OP_CREATE
+    else:
+        globals.OP = OP_DELETE
+
     if args.no_network:
         globals.NO_NETWORK = args.no_network
 
     if args.no_vm:
         globals.NO_VM = args.no_vm
 
     if args.recreate_nw:
```

### Comparing `topology-deployer-0.0.1/deployer/virtual_machine.py` & `topology-deployer-0.0.2/deployer/virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,13 +212,22 @@
         self.__generate_cloud_init_config()
         self.__generate_netplan_config()
         self.__create_root_disk()
         self.__generate_cloud_init_iso()
 
         self.__execute_virt_install_cmd()
 
+    def Delete(self):
+        logging.warning("Deleting Virtual Machine : {}".format(self.name_))
+
+        cmd = "sudo virsh destroy {}".format(self.name_)
+        ExecuteCommand(cmd)
+
+        cmd = "sudo virsh undefine --remove-all-storage {}".format(self.name_)
+        ExecuteCommand(cmd)
+
     def ToString(self) -> str:
         vm_str = ""
         vm_str += "Flavor : {}\n".format(self.flavor_)
         vm_str += "VNC : {}\n".format(self.vnc_port_)
         vm_str += "===================================\n"
         return vm_str
```

### Comparing `topology-deployer-0.0.1/setup.py` & `topology-deployer-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="topology-deployer",
-    version="0.0.1",
+    version="0.0.2",
     author="Ved Patel",
     description=("A python tool to deploy topology "
                 "defined in a json config"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vpatel95/libvirt-topology",
     project_urls={
```

### Comparing `topology-deployer-0.0.1/topology_deployer.egg-info/PKG-INFO` & `topology-deployer-0.0.2/topology_deployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topology-deployer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python tool to deploy topology defined in a json config
 Home-page: https://github.com/vpatel95/libvirt-topology
 Author: Ved Patel
 Project-URL: Bug Tracker, https://github.com/vpatel95/libvirt-topology/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

