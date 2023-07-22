# Comparing `tmp/pydnst-1.0.1.tar.gz` & `tmp/pydnst-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydnst-1.0.1.tar", last modified: Sat Jul 22 12:37:48 2023, max compression
+gzip compressed data, was "pydnst-1.0.2.tar", last modified: Sat Jul 22 12:44:38 2023, max compression
```

## Comparing `pydnst-1.0.1.tar` & `pydnst-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-07-22 12:37:48.062216 pydnst-1.0.1/
--rw-r--r--   0 mm        (1000) mm        (1000)    11357 2020-06-11 21:16:01.000000 pydnst-1.0.1/LICENSE
--rw-rw-r--   0 mm        (1000) mm        (1000)     3314 2023-07-22 12:37:48.062216 pydnst-1.0.1/PKG-INFO
--rw-rw-r--   0 mm        (1000) mm        (1000)     2712 2023-07-22 12:25:22.000000 pydnst-1.0.1/README.md
-drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-07-22 12:37:48.058216 pydnst-1.0.1/pydnst/
--rw-rw-r--   0 mm        (1000) mm        (1000)      721 2023-07-22 10:08:44.000000 pydnst-1.0.1/pydnst/__init__.py
--rw-rw-r--   0 mm        (1000) mm        (1000)     3903 2023-07-22 11:17:11.000000 pydnst-1.0.1/pydnst/__main__.py
--rw-rw-rw-   0 mm        (1000) mm        (1000)    22237 2023-07-22 11:01:33.000000 pydnst-1.0.1/pydnst/client.py
--rw-rw-r--   0 mm        (1000) mm        (1000)     4604 2023-07-22 10:48:50.000000 pydnst-1.0.1/pydnst/commander.py
--rw-rw-r--   0 mm        (1000) mm        (1000)     2569 2022-11-10 10:54:29.000000 pydnst-1.0.1/pydnst/helpers.py
--rw-rw-r--   0 mm        (1000) mm        (1000)    12506 2023-07-22 09:55:25.000000 pydnst-1.0.1/pydnst/message.py
--rw-rw-r--   0 mm        (1000) mm        (1000)    27310 2023-07-22 10:48:27.000000 pydnst-1.0.1/pydnst/server.py
-drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-07-22 12:37:48.062216 pydnst-1.0.1/pydnst.egg-info/
--rw-rw-r--   0 mm        (1000) mm        (1000)     3314 2023-07-22 12:37:48.000000 pydnst-1.0.1/pydnst.egg-info/PKG-INFO
--rw-rw-r--   0 mm        (1000) mm        (1000)      303 2023-07-22 12:37:48.000000 pydnst-1.0.1/pydnst.egg-info/SOURCES.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)        1 2023-07-22 12:37:48.000000 pydnst-1.0.1/pydnst.egg-info/dependency_links.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)       36 2023-07-22 12:37:48.000000 pydnst-1.0.1/pydnst.egg-info/requires.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)        7 2023-07-22 12:37:48.000000 pydnst-1.0.1/pydnst.egg-info/top_level.txt
--rw-rw-r--   0 mm        (1000) mm        (1000)       38 2023-07-22 12:37:48.062216 pydnst-1.0.1/setup.cfg
--rw-rw-r--   0 mm        (1000) mm        (1000)     6865 2023-07-22 12:37:41.000000 pydnst-1.0.1/setup.py
+drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-07-22 12:44:38.986441 pydnst-1.0.2/
+-rw-r--r--   0 mm        (1000) mm        (1000)    11357 2020-06-11 21:16:01.000000 pydnst-1.0.2/LICENSE
+-rw-rw-r--   0 mm        (1000) mm        (1000)     3319 2023-07-22 12:44:38.986441 pydnst-1.0.2/PKG-INFO
+-rw-rw-r--   0 mm        (1000) mm        (1000)     2717 2023-07-22 12:42:38.000000 pydnst-1.0.2/README.md
+drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-07-22 12:44:38.986441 pydnst-1.0.2/pydnst/
+-rw-rw-r--   0 mm        (1000) mm        (1000)      721 2023-07-22 10:08:44.000000 pydnst-1.0.2/pydnst/__init__.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)     3903 2023-07-22 11:17:11.000000 pydnst-1.0.2/pydnst/__main__.py
+-rw-rw-rw-   0 mm        (1000) mm        (1000)    22237 2023-07-22 11:01:33.000000 pydnst-1.0.2/pydnst/client.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)     4604 2023-07-22 10:48:50.000000 pydnst-1.0.2/pydnst/commander.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)     2569 2022-11-10 10:54:29.000000 pydnst-1.0.2/pydnst/helpers.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)    12506 2023-07-22 09:55:25.000000 pydnst-1.0.2/pydnst/message.py
+-rw-rw-r--   0 mm        (1000) mm        (1000)    27310 2023-07-22 10:48:27.000000 pydnst-1.0.2/pydnst/server.py
+drwxrwxr-x   0 mm        (1000) mm        (1000)        0 2023-07-22 12:44:38.986441 pydnst-1.0.2/pydnst.egg-info/
+-rw-rw-r--   0 mm        (1000) mm        (1000)     3319 2023-07-22 12:44:38.000000 pydnst-1.0.2/pydnst.egg-info/PKG-INFO
+-rw-rw-r--   0 mm        (1000) mm        (1000)      303 2023-07-22 12:44:38.000000 pydnst-1.0.2/pydnst.egg-info/SOURCES.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)        1 2023-07-22 12:44:38.000000 pydnst-1.0.2/pydnst.egg-info/dependency_links.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)       36 2023-07-22 12:44:38.000000 pydnst-1.0.2/pydnst.egg-info/requires.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)        7 2023-07-22 12:44:38.000000 pydnst-1.0.2/pydnst.egg-info/top_level.txt
+-rw-rw-r--   0 mm        (1000) mm        (1000)       38 2023-07-22 12:44:38.986441 pydnst-1.0.2/setup.cfg
+-rw-rw-r--   0 mm        (1000) mm        (1000)     6865 2023-07-22 12:42:51.000000 pydnst-1.0.2/setup.py
```

### Comparing `pydnst-1.0.1/LICENSE` & `pydnst-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/PKG-INFO` & `pydnst-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydnst
-Version: 1.0.1
+Version: 1.0.2
 Summary: DNS Tunneling client and server
 Home-page: https://github.com/mori-b/pydnst
 Author: Mori Benech
 Author-email: moribirom@gmail.com
 License: UNKNOWN
 Keywords: dns,tunneling,dns tunneling
 Platform: UNKNOWN
@@ -43,44 +43,44 @@
 Then acquire a DNS name, as short as possible, and configure its nameservers with glue records pointing to your public IP.  
 You can then configure your pydnst.toml field DNST_SERVER_NAME, and run pydnst client on your victim machine.  
 
 
 <a name="usage"></a>
 ## USAGE
 
-###Install the pydnst package on client and server
+### Install the pydnst package on client and server
 
     pip3 install pydnst
     python3 -m pydnst --help
     
-###Generate certificates (recommended), to encrypt the shared key transfer between client and server
+### Generate certificates (recommended), to encrypt the shared key transfer between client and server
 This creates server_private.pem (copy to server) and server_public.pem (copy to client).
 After copying server_private.pem to server, don't forget to chmod 600.
 
     python3 -m pydnst create_certificates
     
-###Generate configuration
+### Generate configuration
 This creates pydnst.toml : edit if needed and then copy to client and server.  
 On client, edit the MAIN_INTERFACE to use the DNS server of this interface, or DNS_SERVER_ADDRESS to circumvent it.  
 On server, edit the LISTENING_INTERFACE.  
 On both, specify the DNST_SERVER_NAME (the DNS name purchased).  
 
     python3 -m pydnst config
     
-###On server
+### On server
 In one terminal, run the server (pydnst.toml must be in the current directory) :   
 Logs are under pydnst.log  
 
     python3 -m pydnst server run
     
 In another terminal, run the commander (pydnst.toml must be in the current directory), which enables to send commands and watch responses in real-time.  
 
     python3 -m pydnst server c2
     
-###On client
+### On client
 In one terminal, run the client (pydnst.toml must be in the current directory) :   
 Logs are under pydnst.log  
 
     python3 -m pydnst client run
```

### Comparing `pydnst-1.0.1/README.md` & `pydnst-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,44 +24,44 @@
 Then acquire a DNS name, as short as possible, and configure its nameservers with glue records pointing to your public IP.  
 You can then configure your pydnst.toml field DNST_SERVER_NAME, and run pydnst client on your victim machine.  
 
 
 <a name="usage"></a>
 ## USAGE
 
-###Install the pydnst package on client and server
+### Install the pydnst package on client and server
 
     pip3 install pydnst
     python3 -m pydnst --help
     
-###Generate certificates (recommended), to encrypt the shared key transfer between client and server
+### Generate certificates (recommended), to encrypt the shared key transfer between client and server
 This creates server_private.pem (copy to server) and server_public.pem (copy to client).
 After copying server_private.pem to server, don't forget to chmod 600.
 
     python3 -m pydnst create_certificates
     
-###Generate configuration
+### Generate configuration
 This creates pydnst.toml : edit if needed and then copy to client and server.  
 On client, edit the MAIN_INTERFACE to use the DNS server of this interface, or DNS_SERVER_ADDRESS to circumvent it.  
 On server, edit the LISTENING_INTERFACE.  
 On both, specify the DNST_SERVER_NAME (the DNS name purchased).  
 
     python3 -m pydnst config
     
-###On server
+### On server
 In one terminal, run the server (pydnst.toml must be in the current directory) :   
 Logs are under pydnst.log  
 
     python3 -m pydnst server run
     
 In another terminal, run the commander (pydnst.toml must be in the current directory), which enables to send commands and watch responses in real-time.  
 
     python3 -m pydnst server c2
     
-###On client
+### On client
 In one terminal, run the client (pydnst.toml must be in the current directory) :   
 Logs are under pydnst.log  
 
     python3 -m pydnst client run
```

### Comparing `pydnst-1.0.1/pydnst/__init__.py` & `pydnst-1.0.2/pydnst/__init__.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst/__main__.py` & `pydnst-1.0.2/pydnst/__main__.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst/client.py` & `pydnst-1.0.2/pydnst/client.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst/commander.py` & `pydnst-1.0.2/pydnst/commander.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst/helpers.py` & `pydnst-1.0.2/pydnst/helpers.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst/message.py` & `pydnst-1.0.2/pydnst/message.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst/server.py` & `pydnst-1.0.2/pydnst/server.py`

 * *Files identical despite different names*

### Comparing `pydnst-1.0.1/pydnst.egg-info/PKG-INFO` & `pydnst-1.0.2/pydnst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydnst
-Version: 1.0.1
+Version: 1.0.2
 Summary: DNS Tunneling client and server
 Home-page: https://github.com/mori-b/pydnst
 Author: Mori Benech
 Author-email: moribirom@gmail.com
 License: UNKNOWN
 Keywords: dns,tunneling,dns tunneling
 Platform: UNKNOWN
@@ -43,44 +43,44 @@
 Then acquire a DNS name, as short as possible, and configure its nameservers with glue records pointing to your public IP.  
 You can then configure your pydnst.toml field DNST_SERVER_NAME, and run pydnst client on your victim machine.  
 
 
 <a name="usage"></a>
 ## USAGE
 
-###Install the pydnst package on client and server
+### Install the pydnst package on client and server
 
     pip3 install pydnst
     python3 -m pydnst --help
     
-###Generate certificates (recommended), to encrypt the shared key transfer between client and server
+### Generate certificates (recommended), to encrypt the shared key transfer between client and server
 This creates server_private.pem (copy to server) and server_public.pem (copy to client).
 After copying server_private.pem to server, don't forget to chmod 600.
 
     python3 -m pydnst create_certificates
     
-###Generate configuration
+### Generate configuration
 This creates pydnst.toml : edit if needed and then copy to client and server.  
 On client, edit the MAIN_INTERFACE to use the DNS server of this interface, or DNS_SERVER_ADDRESS to circumvent it.  
 On server, edit the LISTENING_INTERFACE.  
 On both, specify the DNST_SERVER_NAME (the DNS name purchased).  
 
     python3 -m pydnst config
     
-###On server
+### On server
 In one terminal, run the server (pydnst.toml must be in the current directory) :   
 Logs are under pydnst.log  
 
     python3 -m pydnst server run
     
 In another terminal, run the commander (pydnst.toml must be in the current directory), which enables to send commands and watch responses in real-time.  
 
     python3 -m pydnst server c2
     
-###On client
+### On client
 In one terminal, run the client (pydnst.toml must be in the current directory) :   
 Logs are under pydnst.log  
 
     python3 -m pydnst client run
```

### Comparing `pydnst-1.0.1/setup.py` & `pydnst-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 # To use a consistent encoding
 from codecs import open
 from os import path
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 
 here = path.abspath(path.dirname(__file__))
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as fd:
     long_description = fd.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
```

