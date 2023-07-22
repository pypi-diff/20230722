# Comparing `tmp/oras-0.1.21.tar.gz` & `tmp/oras-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.21.tar", last modified: Thu Jul 20 01:30:32 2023, max compression
+gzip compressed data, was "oras-0.1.22.tar", last modified: Sat Jul 22 14:49:15 2023, max compression
```

## Comparing `oras-0.1.21.tar` & `oras-0.1.22.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.761870 oras-0.1.21/
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-20 01:30:01.000000 oras-0.1.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-20 01:30:01.000000 oras-0.1.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-20 01:30:32.761870 oras-0.1.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5596 2023-07-20 01:30:01.000000 oras-0.1.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.757870 oras-0.1.21/oras/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-20 01:30:01.000000 oras-0.1.21/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-20 01:30:01.000000 oras-0.1.21/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-20 01:30:01.000000 oras-0.1.21/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-20 01:30:01.000000 oras-0.1.21/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-20 01:30:01.000000 oras-0.1.21/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-20 01:30:01.000000 oras-0.1.21/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-20 01:30:01.000000 oras-0.1.21/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.757870 oras-0.1.21/oras/main/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:01.000000 oras-0.1.21/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-20 01:30:01.000000 oras-0.1.21/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-20 01:30:01.000000 oras-0.1.21/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (122)    35813 2023-07-20 01:30:01.000000 oras-0.1.21/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-20 01:30:01.000000 oras-0.1.21/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.757870 oras-0.1.21/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/artifact.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.757870 oras-0.1.21/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-20 01:30:01.000000 oras-0.1.21/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.761870 oras-0.1.21/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-20 01:30:01.000000 oras-0.1.21/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-07-20 01:30:01.000000 oras-0.1.21/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-20 01:30:01.000000 oras-0.1.21/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-20 01:30:01.000000 oras-0.1.21/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 01:30:32.757870 oras-0.1.21/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-20 01:30:32.000000 oras-0.1.21/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-20 01:30:32.000000 oras-0.1.21/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 01:30:32.000000 oras-0.1.21/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 01:30:28.000000 oras-0.1.21/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-20 01:30:32.000000 oras-0.1.21/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-20 01:30:32.000000 oras-0.1.21/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-20 01:30:01.000000 oras-0.1.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-20 01:30:32.761870 oras-0.1.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-20 01:30:01.000000 oras-0.1.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-22 14:48:49.000000 oras-0.1.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-22 14:48:49.000000 oras-0.1.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-22 14:49:15.163141 oras-0.1.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5596 2023-07-22 14:48:49.000000 oras-0.1.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.155141 oras-0.1.22/oras/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-22 14:48:49.000000 oras-0.1.22/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-22 14:48:49.000000 oras-0.1.22/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-07-22 14:48:49.000000 oras-0.1.22/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-22 14:48:49.000000 oras-0.1.22/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-22 14:48:49.000000 oras-0.1.22/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-22 14:48:49.000000 oras-0.1.22/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-22 14:48:49.000000 oras-0.1.22/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.159141 oras-0.1.22/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 14:48:49.000000 oras-0.1.22/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-22 14:48:49.000000 oras-0.1.22/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-22 14:48:49.000000 oras-0.1.22/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35967 2023-07-22 14:48:49.000000 oras-0.1.22/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-22 14:48:49.000000 oras-0.1.22/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/artifact.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-22 14:48:49.000000 oras-0.1.22/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.163141 oras-0.1.22/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-22 14:48:49.000000 oras-0.1.22/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10818 2023-07-22 14:48:49.000000 oras-0.1.22/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-07-22 14:48:49.000000 oras-0.1.22/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-22 14:48:49.000000 oras-0.1.22/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:49:15.159141 oras-0.1.22/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-22 14:49:15.000000 oras-0.1.22/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:49:10.000000 oras-0.1.22/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-22 14:49:14.000000 oras-0.1.22/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-22 14:48:49.000000 oras-0.1.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-22 14:49:15.163141 oras-0.1.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-22 14:48:49.000000 oras-0.1.22/setup.py
```

### Comparing `oras-0.1.21/LICENSE` & `oras-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/PKG-INFO` & `oras-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.21
+Version: 0.1.22
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.21 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.22 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
```

### Comparing `oras-0.1.21/README.md` & `oras-0.1.22/README.md`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/auth.py` & `oras-0.1.22/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/client.py` & `oras-0.1.22/oras/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,28 +26,29 @@
     """
 
     def __init__(
         self,
         hostname: Optional[str] = None,
         registry: Optional[oras.provider.Registry] = None,
         insecure: bool = False,
+        tls_verify: bool = True,
     ):
         """
         Create an ORAS client.
 
         The hostname is the remote registry to ping.
 
         :param hostname: the hostname of the registry to ping
         :type hostname: str
         :param registry: if provided, use this custom provider instead of default
         :type registry: oras.provider.Registry or None
         :param insecure: use http instead of https
         :type insecure: bool
         """
-        self.remote = registry or oras.provider.Registry(hostname, insecure)
+        self.remote = registry or oras.provider.Registry(hostname, insecure, tls_verify)
 
     def __repr__(self) -> str:
         return str(self)
 
     def __str__(self) -> str:
         return "[oras-client]"
 
@@ -138,14 +139,15 @@
 
     def login(
         self,
         username: str,
         password: str,
         password_stdin: bool = False,
         insecure: bool = False,
+        tls_verify: bool = True,
         hostname: Optional[str] = None,
         config_path: Optional[List[str]] = None,
     ) -> dict:
         """
         Login to a registry.
 
         :param registry: if provided, use this custom provider instead of default
@@ -154,27 +156,29 @@
         :type username: str
         :param password: the user account password
         :type password: str
         :param password_stdin: get the password from standard input
         :type password_stdin: bool
         :param insecure: use http instead of https
         :type insecure: bool
+        :param tls_verify: verify tls
+        :type tls_verify: bool
         :param hostname: the hostname to login to
         :type hostname: str
         :param config_path: list of config paths to add
         :type config_path: list
         """
         login_func = self._login
         if hasattr(self.remote, "login"):
             login_func = self.remote.login  # type: ignore
         return login_func(
             username=username,
             password=password,
             password_stdin=password_stdin,
-            insecure=insecure,
+            tls_verify=tls_verify,
             hostname=hostname,
             config_path=config_path,  # type: ignore
         )
 
     def logout(self, hostname: str):
         """
         Logout from a registry, meaning removing any auth (if loaded)
@@ -185,15 +189,15 @@
         self.remote.logout(hostname)
 
     def _login(
         self,
         username: Optional[str] = None,
         password: Optional[str] = None,
         password_stdin: bool = False,
-        insecure: bool = False,
+        tls_verify: bool = True,
         hostname: Optional[str] = None,
         config_path: Optional[str] = None,
     ) -> dict:
         """
         Login to an OCI registry.
 
         The username and password can come from stdin. Most people use username
@@ -220,15 +224,15 @@
 
         # Set basic auth for the client
         self.set_basic_auth(username, password)
 
         # Login
         # https://docker-py.readthedocs.io/en/stable/client.html?highlight=login#docker.client.DockerClient.login
         try:
-            client = oras.utils.get_docker_client(insecure=insecure)
+            client = oras.utils.get_docker_client(tls_verify=tls_verify)
             return client.login(
                 username=username,
                 password=password,
                 registry=hostname,
                 dockercfg_path=config_path,
             )
```

### Comparing `oras-0.1.21/oras/container.py` & `oras-0.1.22/oras/container.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/decorator.py` & `oras-0.1.22/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/defaults.py` & `oras-0.1.22/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/logger.py` & `oras-0.1.22/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/main/login.py` & `oras-0.1.22/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/oci.py` & `oras-0.1.22/oras/oci.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/provider.py` & `oras-0.1.22/oras/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,33 +27,40 @@
     """
     Direct interactions with an OCI registry.
 
     This could also be called a "provider" when we add in the "copy" logic
     and the registry isn't necessarily the "remote" endpoint.
     """
 
-    def __init__(self, hostname: Optional[str] = None, insecure: bool = False):
+    def __init__(
+        self,
+        hostname: Optional[str] = None,
+        insecure: bool = False,
+        tls_verify: bool = True,
+    ):
         """
         Create a new registry provider.
 
         :param hostname: the registry hostname (optional)
         :type hostname: str
         :param insecure: use http instead of https
         :type insecure: bool
+        :param tls_verify: verify TLS certificates
+        :type tls_verify: bool
         """
         self.hostname: Optional[str] = hostname
         self.headers: dict = {}
         self.session: requests.Session = requests.Session()
         self.prefix: str = "http" if insecure else "https"
         self.token: Optional[str] = None
         self._auths: dict = {}
         self._basic_auth = None
-        self._insecure = insecure
+        self._tls_verify = tls_verify
 
-        if insecure:
+        if not tls_verify:
             requests.packages.urllib3.disable_warnings()  # type: ignore
 
     def logout(self, hostname: str):
         """
         If auths are loaded, remove a hostname.
 
         :param hostname: the registry hostname to remove
@@ -842,15 +849,15 @@
         response = self.session.request(
             method,
             url,
             data=data,
             json=json,
             headers=headers,
             stream=stream,
-            verify=not self._insecure,
+            verify=self._tls_verify,
         )
 
         # A 401 response is a request for authentication
         if response.status_code not in [401, 404]:
             return response
 
         # Otherwise, authenticate the request and retry
```

### Comparing `oras-0.1.21/oras/schemas.py` & `oras-0.1.22/oras/schemas.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/tests/test_oras.py` & `oras-0.1.22/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/tests/test_provider.py` & `oras-0.1.22/oras/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/tests/test_utils.py` & `oras-0.1.22/oras/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/utils/fileio.py` & `oras-0.1.22/oras/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/oras/utils/request.py` & `oras-0.1.22/oras/utils/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     query = dict(urlparse.parse_qsl(parts.query))
     query.update(params)
     updated = list(parts)
     updated[4] = urlencode(query)
     return urlparse.urlunparse(updated)
 
 
-def get_docker_client(insecure: bool = False, **kwargs):
+def get_docker_client(tls_verify: bool = True, **kwargs):
     """
     Get a docker client.
 
-    :param tls : enable tls
-    :type tls: bool
+    :param tls_verify : enable tls
+    :type tls_verify: bool
     """
     import docker
 
-    return docker.DockerClient(tls=not insecure, **kwargs)
+    return docker.DockerClient(tls=tls_verify, **kwargs)
```

### Comparing `oras-0.1.21/oras/version.py` & `oras-0.1.22/oras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.21"
+__version__ = "0.1.22"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.21/oras.egg-info/PKG-INFO` & `oras-0.1.22/oras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.21
+Version: 0.1.22
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.21 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.22 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
```

### Comparing `oras-0.1.21/oras.egg-info/SOURCES.txt` & `oras-0.1.22/oras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oras-0.1.21/setup.py` & `oras-0.1.22/setup.py`

 * *Files identical despite different names*

