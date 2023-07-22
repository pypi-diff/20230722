# Comparing `tmp/port_pulumi-1.1.0.tar.gz` & `tmp/port_pulumi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_pulumi-1.1.0.tar", last modified: Thu Jul 20 12:37:50 2023, max compression
+gzip compressed data, was "port_pulumi-1.1.1.tar", last modified: Sat Jul 22 11:47:06 2023, max compression
```

## Comparing `port_pulumi-1.1.0.tar` & `port_pulumi-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.054244 port_pulumi-1.1.0/port_pulumi/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98686 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/port_pulumi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    79853 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/port_pulumi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/port_pulumi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 12:37:50.000000 port_pulumi-1.1.0/port_pulumi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:37:50.058244 port_pulumi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-20 12:37:49.000000 port_pulumi-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/port_pulumi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98686 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36131 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34831 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/port_pulumi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22683 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79853 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/port_pulumi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/port_pulumi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 11:47:06.652286 port_pulumi-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-22 11:47:06.000000 port_pulumi-1.1.1/setup.py
```

### Comparing `port_pulumi-1.1.0/PKG-INFO` & `port_pulumi-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port_pulumi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -50,14 +50,14 @@
 go get github.com/port-labs/pulumi-port/sdk
 ```
 
 ## Configuration
 
 The following configuration points are available for the `port` provider:
 
-- `port:clientId` - This is the Port client ID.
-- `port:secret` - This is the Port secret.
-- `port:baseUrl` (optional) - This is the Port base URL.
+- `port:clientId` - This is the Port client ID. (environment: PORT_CLIENT_ID)
+- `port:secret` - This is the Port secret. (environment: PORT_CLIENT_SECRET)
+- `port:baseUrl` (optional) - This is the Port base URL. (environment: PORT_BASE_URL)
 - `port:token` - (optional) This is the Port token.
```

### Comparing `port_pulumi-1.1.0/README.md` & `port_pulumi-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 go get github.com/port-labs/pulumi-port/sdk
 ```
 
 ## Configuration
 
 The following configuration points are available for the `port` provider:
 
-- `port:clientId` - This is the Port client ID.
-- `port:secret` - This is the Port secret.
-- `port:baseUrl` (optional) - This is the Port base URL.
+- `port:clientId` - This is the Port client ID. (environment: PORT_CLIENT_ID)
+- `port:secret` - This is the Port secret. (environment: PORT_CLIENT_SECRET)
+- `port:baseUrl` (optional) - This is the Port base URL. (environment: PORT_BASE_URL)
 - `port:token` - (optional) This is the Port token.
```

### Comparing `port_pulumi-1.1.0/port_pulumi/__init__.py` & `port_pulumi-1.1.1/port_pulumi/__init__.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/_inputs.py` & `port_pulumi-1.1.1/port_pulumi/_inputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/_utilities.py` & `port_pulumi-1.1.1/port_pulumi/_utilities.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/action.py` & `port_pulumi-1.1.1/port_pulumi/action.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/blueprint.py` & `port_pulumi-1.1.1/port_pulumi/blueprint.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/config/vars.py` & `port_pulumi-1.1.1/port_pulumi/config/vars.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/entity.py` & `port_pulumi-1.1.1/port_pulumi/entity.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/outputs.py` & `port_pulumi-1.1.1/port_pulumi/outputs.py`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/port_pulumi/provider.py` & `port_pulumi-1.1.1/port_pulumi/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,65 +10,67 @@
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
-                 client_id: pulumi.Input[str],
-                 secret: pulumi.Input[str],
                  base_url: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 secret: Optional[pulumi.Input[str]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] client_id: Client ID for Port-labs
         :param pulumi.Input[str] secret: Client Secret for Port-labs
         :param pulumi.Input[str] token: Token for Port-labs
         """
-        pulumi.set(__self__, "client_id", client_id)
-        pulumi.set(__self__, "secret", secret)
         if base_url is not None:
             pulumi.set(__self__, "base_url", base_url)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if secret is not None:
+            pulumi.set(__self__, "secret", secret)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
+    @pulumi.getter(name="baseUrl")
+    def base_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "base_url")
+
+    @base_url.setter
+    def base_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "base_url", value)
+
+    @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Input[str]:
+    def client_id(self) -> Optional[pulumi.Input[str]]:
         """
         Client ID for Port-labs
         """
         return pulumi.get(self, "client_id")
 
     @client_id.setter
-    def client_id(self, value: pulumi.Input[str]):
+    def client_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_id", value)
 
     @property
     @pulumi.getter
-    def secret(self) -> pulumi.Input[str]:
+    def secret(self) -> Optional[pulumi.Input[str]]:
         """
         Client Secret for Port-labs
         """
         return pulumi.get(self, "secret")
 
     @secret.setter
-    def secret(self, value: pulumi.Input[str]):
+    def secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret", value)
 
     @property
-    @pulumi.getter(name="baseUrl")
-    def base_url(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "base_url")
-
-    @base_url.setter
-    def base_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "base_url", value)
-
-    @property
     @pulumi.getter
     def token(self) -> Optional[pulumi.Input[str]]:
         """
         Token for Port-labs
         """
         return pulumi.get(self, "token")
 
@@ -99,15 +101,15 @@
         :param pulumi.Input[str] secret: Client Secret for Port-labs
         :param pulumi.Input[str] token: Token for Port-labs
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProviderArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The provider type for the port package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
@@ -136,19 +138,15 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["base_url"] = base_url
-            if client_id is None and not opts.urn:
-                raise TypeError("Missing required property 'client_id'")
             __props__.__dict__["client_id"] = client_id
-            if secret is None and not opts.urn:
-                raise TypeError("Missing required property 'secret'")
             __props__.__dict__["secret"] = None if secret is None else pulumi.Output.secret(secret)
             __props__.__dict__["token"] = None if token is None else pulumi.Output.secret(token)
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["secret", "token"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'port',
             resource_name,
@@ -158,23 +156,23 @@
     @property
     @pulumi.getter(name="baseUrl")
     def base_url(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "base_url")
 
     @property
     @pulumi.getter(name="clientId")
-    def client_id(self) -> pulumi.Output[str]:
+    def client_id(self) -> pulumi.Output[Optional[str]]:
         """
         Client ID for Port-labs
         """
         return pulumi.get(self, "client_id")
 
     @property
     @pulumi.getter
-    def secret(self) -> pulumi.Output[str]:
+    def secret(self) -> pulumi.Output[Optional[str]]:
         """
         Client Secret for Port-labs
         """
         return pulumi.get(self, "secret")
 
     @property
     @pulumi.getter
```

### Comparing `port_pulumi-1.1.0/port_pulumi.egg-info/PKG-INFO` & `port_pulumi-1.1.1/port_pulumi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-pulumi
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Pulumi package for creating and managing Port resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/port-labs/pulumi-port
 Keywords: pulumi port category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -50,14 +50,14 @@
 go get github.com/port-labs/pulumi-port/sdk
 ```
 
 ## Configuration
 
 The following configuration points are available for the `port` provider:
 
-- `port:clientId` - This is the Port client ID.
-- `port:secret` - This is the Port secret.
-- `port:baseUrl` (optional) - This is the Port base URL.
+- `port:clientId` - This is the Port client ID. (environment: PORT_CLIENT_ID)
+- `port:secret` - This is the Port secret. (environment: PORT_CLIENT_SECRET)
+- `port:baseUrl` (optional) - This is the Port base URL. (environment: PORT_BASE_URL)
 - `port:token` - (optional) This is the Port token.
```

### Comparing `port_pulumi-1.1.0/port_pulumi.egg-info/SOURCES.txt` & `port_pulumi-1.1.1/port_pulumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `port_pulumi-1.1.0/setup.py` & `port_pulumi-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.0"
-PLUGIN_VERSION = "1.1.0"
+VERSION = "1.1.1"
+PLUGIN_VERSION = "1.1.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'port', PLUGIN_VERSION, '--server', 'github://api.github.com/port-labs/pulumi-port'])
         except OSError as error:
```

